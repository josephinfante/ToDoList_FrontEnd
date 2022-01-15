<template>
  <header class="bg-gray-900 text-white py-5">
    <div class="container mx-auto px-5 flex grid grid-cols-2 gap-4">
      <div>Logo</div>
      <div class="flex justify-end">
        <a href="" class="mx-3">Iniciar sesión</a>
        <a href="" class="mx-3">Registrarse</a>
        <label class="switch ml-3">
          <input type="checkbox">
          <span class="slider round"></span>
        </label>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<style>
.switch {
  position: relative;
  display: inline-block;
  width: 60px;
  height: 34px;
}

.switch input { 
  opacity: 0;
  width: 0;
  height: 0;
}

.slider {
  position: absolute;
  cursor: pointer;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #FCFC62;
  -webkit-transition: .4s;
  transition: .4s;
}

.slider:before {
  position: absolute;
  content: "";
  height: 26px;
  width: 26px;
  left: 4px;
  bottom: 4px;
  background-color: white;
  -webkit-transition: .4s;
  transition: .4s;
}

input:checked + .slider {
  background-color: #2D3047;
}

input:focus + .slider {
  box-shadow: 0 0 1px #2D3047;
}

input:checked + .slider:before {
  -webkit-transform: translateX(26px);
  -ms-transform: translateX(26px);
  transform: translateX(26px);
}

/* Rounded sliders */
.slider.round {
  border-radius: 34px;
}

.slider.round:before {
  border-radius: 50%;
}
</style>