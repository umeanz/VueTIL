# Vue.js Study 
WhY using the 'vue.js'?!
- Vue.js is progressive framework 
- Oringinal way to update web is that developer have update a data to DOM. However the 'Vue.js' checking the reactivility MOdel-VIe-VIewMOdel(MVVM)<br/>
*if keep changing DOM, the count of redering is increasing. 
- fast HTML rendering.
- Keep version up.
- Web-app
- Easy syntax
- the way to code is already set in only one way(syntax
)
- Ptential Framework
<br/>
<br/>
<br/>

## Basic form sytax
---------------------------------------------------
```vue
<template>
...
</template>

<script>
....
</script>

<style>
...
</style>
```

## syntax
----------------------------------------------------
1) Instanse & Life cycle
2) Computed
3) Computed chache
4) Getter, Setter
5) Watch 
6) class & style binding 
    - v-bind: is make in shot :
    - v-bind:class="{keyvalue: kevlaue2}" -> when keyvalue2 is true, keyvalue class generated. 
    - dont have to be line data. Can be object data
    - style binding is better to do in direct
    ``` 
    <div :style="styleObject"></div>

    <script>
    export default { 
        data(){
            styleObject: {
                color: 'red',
                fontSize:'12px' //camelCase
            }
        }
    }
    ```
    - when put two object in style can use array style.

7) conditioning rendering 
    - v-if use redering a block up to condtion. 
    - v-show is always rendering, even not match with initial condition.<br/>(Firt, v-show redering element in DOM(html). and follow the condition change CSS propeety display:block/display:none)
    - generaly v-if has higher toggle cost while v-show has higher initial render costs.(from vuejs.org)<br/> the v-show better to use change toggle often or it is better yo use v-if as not change condition in runtime. 

8) List rendering<br/>
    (key need specific value) 
    