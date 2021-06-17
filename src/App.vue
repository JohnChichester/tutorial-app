<template>
  <div id="app" class="small-container">
    <h1>Employees</h1>
    <employee-table />
    <employee-table :employees="employees" />
  </div>
</template>

<script>
import EmployeeTable from "./components/EmployeeTable.vue";

export default {
  name: "App",
  components: {
    EmployeeTable,
  },
  data() {
    return {
      employees: [
        {
          id: 1,
          name: "Richard Hendricks",
          email: "richard@test.com",
        },
        {
          id: 2,
          name: "Bertram Gilfoyle",
          email: "bertram@test.com",
        },
        {
          id: 3,
          name: "Dinnah Cat",
          email: "dinnahcat@test.com",
        },
      ],
    };
  },
};
</script>

<style>
#app {
  button {
    background: #009555;
    border: 1px solid #009999;
  }
  .snall-container {
    max-width: 680px;
    margin: auto;
  }
}
</style>
