<template>
  <div class="Search">
    <input type="text" class="Search__input">
    <button class="Search__button">
      <i class="fa fa-search"></i>
    </button>
  </div>
</template>

<style>
.Search {
  display: flex;
  justify-content: center;
  padding: 99px 18px;
}

.Search__input {
  color: #fff;
  background: #262626;
  border: 1px solid #b7b7b7;
  width: 437px;
  height: 53px;
  font-size: 32px;
  padding: 17px;
  outline: none;
}

.Search__button {
  background: #262626;
  border: 1px solid #b7b7b7;
  color: #fff;
  padding: 10px 12px;
  transition: all 0.2s ease-in-out;
}

.Search__button:hover {
  background: #b7b7b7;
  color: #262626;
}
</style>

