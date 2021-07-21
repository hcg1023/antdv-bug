<template>
  <a-table
    bordered
    :data-source="[{}, {}]"
    :columns="columns"
    :scroll="{
      x: columns.length * 160,
      y: false
    }"
  >
  </a-table>
</template>

<script>
export default {
  name: "App",
  components: {},
  setup() {
    const columns = [
      {
        title: "Full Name",
        width: "100px",
        dataIndex: "name",
        key: "name",
        fixed: "left"
      },
      {
        title: "Age",
        width: "80px",
        dataIndex: "age",
        key: "age"
      },
      { title: "Column 1", width: "80px", dataIndex: "address", key: "1" },
      { title: "Column 2", width: "80px", dataIndex: "address", key: "2" },
      { title: "Column 3", width: "80px", dataIndex: "address", key: "3" },
      { title: "Column 4", width: "80px", dataIndex: "address", key: "4" },
      { title: "Column 5", width: "80px", dataIndex: "address", key: "5" },
      { title: "Column 6", width: "80px", dataIndex: "address", key: "6" },
      { title: "Column 7", width: "80px", dataIndex: "address", key: "7" },
      { title: "Column 8", width: "80px", dataIndex: "address", key: "8" },
      {
        title: "Action",
        key: "operation",
        fixed: "right",
        width: 100
      }
    ];

    return {
      columns
    };
  }
};
</script>
