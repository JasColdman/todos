Примеры запросов в среде `GraphiQL`

```
mutation createTodo {
  createTodo(input: { text: "first todo", userId: "1" }) {
    user {
      id
      name
    }
    text
    done
  }
}

query findTodos {
  todos {
    text
    done
    user {
      name
    }
  }
}
```