<template>
    <header>
        <div class="language-menu">
            <div class="language-menu-item">
                <!-- <span>Language</span> -->
            </div>
            <div class="language-menu-item switcher-wrapper">
                <div class="lang">eng</div>
                <div>
                    <label class="switch">
                        <input type="checkbox">
                        <span class="slider round"></span>
                    </label>
                </div>
                <div class="lang">tur</div>
            </div>
            <div class="language-menu-item">
                <div class="language-menu-item-pass"></div>
            </div>
        </div>
    </header>
</template>


<script>

export default {

}
</script>

<style scoped>

header {
    height: 72px;
    color: #fff;
}


.language-menu {
    display: flex;
    justify-content: flex-end;
}

.switcher-wrapper {
    display: flex;
}

.lang {
    padding: 0 1em;
    font-size: .95em;
}

.language-menu-item {
    line-height: 72px;
    padding: 0 1em;
}

.language-menu-item span {
    font-size: .9em;
}

/* The switch - the box around the slider */
.switch {
  position: relative;
  display: inline-block;
  margin-top: 24px;
  width: 40px;
  height: 22px;
}

/* Hide default HTML checkbox */
.switch input {
  opacity: 0;
  width: 0;
  height: 0;
}

/* The slider */
.slider {
  position: absolute;
  cursor: pointer;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #ccc;
  -webkit-transition: .4s;
  transition: .4s;
}

.slider:before {
  position: absolute;
  content: "";
  height: 17px;
  width: 17px;
  left: 3px;
  bottom: 3px;
  background-color: white;
  -webkit-transition: .4s;
  transition: .4s;
}

input:checked + .slider {
  /background-color: #2196F3;
}

input:focus + .slider {
  box-shadow: 0 0 1px #2196F3;
}

input:checked + .slider:before {
  -webkit-transform: translateX(17px);
  -ms-transform: translateX(17px);
  transform: translateX(17px);
}

/* Rounded sliders */
.slider.round {
  border-radius: 11px;
}

.slider.round:before {
  border-radius: 50%;
}

</style>

