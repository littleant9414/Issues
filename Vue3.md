# 🔎 Vue3

## 🔺 Issue

🔸 watch

  ```javascript
    //  issue :
    when click button console log shows below
    => person change Proxy {name: "jack!!!", age: 19} Proxy {name: "jack!!!", age: 19}

    <template>
      <div>
        <h2>name : {{ person.name }}</h2>
        <h2>age : {{ person.age }}</h2>
        <button @click="person.name += '!'">edit name</button>
      </div>
    </template>

    <script>
      import { reactive, ref, watch } from "vue"

      export default {
        name: "Demo",
        setup() {
          let person = ref({
            name: "jack",
            age: 19,
          })
          watch(person.value, (newvalue, oldvalue) => {
            console.log("person change", newvalue, oldvalue)
          })
          return {
            person,
          }
        },
      }
    </script>

    // solutioin : 
    if really need the oldvalue and newValue use ref to monitor data
    => let age = ref(18)
  ```

