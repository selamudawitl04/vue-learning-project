<template>
    <button class="my-button">{{ buttonText }}</button>
</template>

<script>
    export default{
        name: 'MyButton',
        props: {
            buttonText: String
        }
    }
</script>
<style>
.my-button{
    font: inherit;
    border: 1px solid #88005b;
    background-color: #88005b;
    color: white;
    padding: 1rem 2rem;
    border-radius: 12px;
    margin: 1rem;
    width: 12rem;
    cursor: pointer;
    box-shadow: 1px 1px 4px rgba(0, 0, 0, 0.26);
}
.my-button:focus {
    outline: none;
  }
  .my-button:hover,
  .my-button:active {
    background-color: #af0a78;
    border-color: #af0a78;
    box-shadow: 1px 1px 8px rgba(0, 0, 0, 0.26);
  }
  .my-button:disabled {
    background-color: #ccc;
    border-color: #ccc;
    box-shadow: none;
    color: #3f3f3f;
    cursor: not-allowed;
  }
</style>