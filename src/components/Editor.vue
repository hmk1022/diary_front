<template>
    <div id="app"> 
        <button @click="test()">test</button>
        <vue-editor  v-model="htmlForEditor" :editorToolbar="customToolbar" ></vue-editor>
    </div>
</template>

<script>
import { VueEditor } from 'vue2-quill-editor'

export default {
    name : 'Editor',
    components: { VueEditor },

    data() {
        return {
            htmlForEditor: null ,
            customToolbar: [
                ['bold', 'italic', 'underline'],
                [{ 'list': 'ordered'}, { 'list': 'bullet' }],
                ['image', 'code-block']
            ]
        }
    },

    methods: {
        setEditorContent: function() {
            this.htmlForEditor = '<h1>Html For Editor</h1>'
        },
        searchChangeFunc(e){
            console.log(e.target.value)
        },
        test (){
            console.log("에디터 텍스트 : ",this.htmlForEditor)
        }
    }
    
}
</script>