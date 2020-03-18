<template>
    <editor
    :value="editorText"
    :options="editorOptions"
    :html="editorHtml"
    :visible="editorVisible"
    previewStyle="vertical"
    height="500px"
    mode="wysiwyg"
    />
</template>

<script>
import 'tui-editor/dist/tui-editor.css';
import 'tui-editor/dist/tui-editor-contents.css';
import 'codemirror/lib/codemirror.css';
import { Editor } from '@toast-ui/vue-editor'


export default {
  name: 'TextEditor',
  data (){
      return {
          editorText: '',
          editorOptions: {
            minHeight: '200px',
            language: 'en_US',
            useCommandShortcut: true,
            useDefaultHTMLSanitizer: true,
            usageStatistics: true,
            hideModeSwitch: false,
            toolbarItems: [
                'heading',
                'bold',
                'italic',
                'strike',
                'divider',
                'hr',
                'quote',
                'divider',
                'ul',
                'ol',
                'task',
                'indent',
                'outdent',
                'divider',
                'table',
                'image',
                'link',
                'divider',
                'code',
                'codeblock'
            ]
        },
        editorHtml: '',
        editorVisible: true
      }
  },
  components: {
      editor: Editor
  }
}
</script>