<script>
  import Announcement from "./Announcement.svelte";
  import Button from "./Button.svelte";

  let fruits = [
    { name: "apple", color: "red", amount: 5, id: 1 },
    { name: "banana", color: "yellow", amount: 1, id: 2 },
    { name: "grape", color: "blue", amount: 14, id: 3 },
  ];

  const deleteFruit = (id) => {
    fruits = fruits.filter((fruit) => fruit.id != id);
    console.log(fruits);
  };
</script>

<main>
  <Button btnText={"Bye friend"} />
</main>

<style>
  h5,
  p {
    margin: 4px 0px;
  }

  .card {
    padding: 8px;
    border-radius: 20px;
    border: 2px solid gray;
    min-width: 400px;
  }

  main {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  h1 {
    text-align: center;
  }
</style>
