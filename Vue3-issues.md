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
          let person = reactive({
            name: "jack",
            age: 19,
          })
          watch(person, (newvalue, oldvalue) => {
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

  🔸 watch (deep config forced on)

  ```javascript
    //  issue :
    { deep: false } => console log shows below
    =>  [[Handler]]: Object
        [[Target]]: Object
        age: 19
        job:
        salary: 3001
        [[Prototype]]: Object
        name: "jack"
        [[Prototype]]: Object
        [[IsRevoked]]: false


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
          let person = reactive({
            name: "jack",
            age: 19,
          })
          watch(person, (newvalue, oldvalue) => {
            console.log("person change", newvalue, oldvalue)
          },{ deep: false })
          return {
            person,
          }
        },
      }
    </script>
  ```
