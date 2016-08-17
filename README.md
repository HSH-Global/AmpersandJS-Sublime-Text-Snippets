# AmpersandJS Code Snippets

[![JavaScript Style Guide](https://cdn.rawgit.com/feross/standard/master/badge.svg)](https://github.com/feross/standard)

Snippets to create faster and better [AmpersandJS](https://ampersandjs.com/) JavaScript apps. 

## Snippets

To use a snippet, type the trigger codes (listed below in bold) then hit `tab` or `ctrl + enter`.
*Remember*, you can press `tab` / `shift + tab` for speedy navigation from one part of the code to another.

### [Ampersand initialize](https://ampersandjs.com/docs/#ampersand-state-constructorinitialize) function

**Trigger:** initialize

```xml
<snippet>
  <content><![CDATA[
initialize: function (${1:opts}) {
  var ${2:self} = this    
},
]]></content>
  <tabTrigger>initialize</tabTrigger>
  <scope>source.js, source.jsx, source.ts</scope>
  <description>Ampersand initialize function</description>
</snippet>
```

### General [Ampersand-State](https://ampersandjs.com/docs/#ampersand-state-extend) extend

**Trigger:** ampersandState

```xml
<snippet>
  <content><![CDATA[
var AmpersandModel = require('ampersand-model')

module.exports = AmpersandModel.extend({
  extraProperties: ${1:'ignore'},
  props: {
    ${2:}
  },
  session: {
    ${3:}
  },
  derived: {
    ${4:}
  }
})
]]></content>
  <tabTrigger>ampersandState</tabTrigger>
  <scope>source.js, source.jsx, source.ts</scope>
  <description>Ampersand State</description>
</snippet>
```

### [Ampersand derived property](https://ampersandjs.com/docs/#ampersand-state-derived) definition

**Trigger:** deps

```xml
<snippet>
  <content><![CDATA[
deps: ['${1:property}'],
fn: function () {
  ${2:}
},
cache: ${3:true}
]]></content>
  <tabTrigger>deps</tabTrigger>
  <scope>source.js, source.jsx, source.ts</scope>
  <description>derived property</description>
</snippet>
```

### [Ampersand props property](https://ampersandjs.com/docs/#ampersand-state-props) definition

**Trigger:** prop

```xml
<snippet>
  <content><![CDATA[
${1:prop}: {
  type: '${2:string}',
  required: ${3:true},
  default: '${4:}', 
  values: ['${5:}'],
  allowNull: ${6:false},
  setOnce: ${7:false}
}
]]></content>
  <tabTrigger>prop</tabTrigger>
  <scope>source.js, source.jsx, source.ts</scope>
  <description>State props property</description>
</snippet>
```

### General [Ampersand-Model](https://ampersandjs.com/docs/#ampersand-model-extend) extend

**Trigger:** ampersandModel

```xml
<snippet>
  <content><![CDATA[
var AmpersandModel = require('ampersand-model')

module.exports = AmpersandModel.extend({
  ajaxConfig: function () {
    var model = this
    return {
      headers: {
      
      },
      xhrFields: {
      
      }
    }
  },
  url: function () {
    var model = this

    return model.urlRoot
  },
  urlRoot: '',
  props: {},
  session: {},
  derived: {}
})
]]></content>
  <tabTrigger>ampersandModel</tabTrigger>
  <scope>source.js, source.jsx, source.ts</scope>
  <description>Ampersand Model</description>
</snippet>
```

### General [Ampersand-Rest-Collection](https://ampersandjs.com/docs/#ampersand-collection-extend) extend

**Trigger:** ampersandCollection

```xml
<snippet>
  <content><![CDATA[
var AmpersandRestCollection = require('ampersand-rest-collection')
var ${1:Model} = require('${2:../models/${3:}}')

module.exports = AmpersandRestCollection.extend({
  model: ${1:Model},
  mainIndex: '${4:_id}',
  url: '${5:}'
})

]]></content>
  <tabTrigger>ampersandCollection</tabTrigger>
  <scope>source.js, source.jsx, source.ts</scope>
  <description>Ampersand REST Collection</description>
</snippet>
```

### General [Ampersand-View](https://ampersandjs.com/docs/#ampersand-view-extend) extend

**Trigger:** ampersandView

```xml
<snippet>
  <content><![CDATA[
var AmpersandView = require('ampersand-view')

module.exports = AmpersandView.extend({
  template: function () {},
  events: {

  },
  bindings: {

  }
})

]]></content>
  <tabTrigger>ampersandView</tabTrigger>
  <scope>source.js, source.jsx, source.ts</scope>
  <description>Ampersand View</description>
</snippet>
```

### Simple [Ampersand bindings](https://ampersandjs.com/docs/#ampersand-view-bindings) declaration

**Trigger:** model.

```xml
<snippet>
  <content><![CDATA[
'model.${1:name}': {
  type: '${2:text}',
  selector: '${3:[data-hook="${4:name}"]}'
}
]]></content>
  <tabTrigger>model.</tabTrigger>
  <scope>source.js, source.jsx, source.ts</scope>
  <description>model binding property</description>
</snippet>
```

### [registerSubview](https://ampersandjs.com/docs/#ampersand-view-registersubview) function

**Trigger:** registerSubview

```xml
<snippet>
  <content><![CDATA[
view.registerSubview(${1:viewInstance})
]]></content>
  <tabTrigger>registerSubview</tabTrigger>
  <scope>source.js, source.jsx, source.ts</scope>
  <description>registerSubview function</description>
</snippet>
```

### [render](https://ampersandjs.com/docs/#ampersand-view-render) function

**Trigger:** render

```xml
<snippet>
  <content><![CDATA[
render: function (${1:opts}) {
  var view = this
  ${2:view._upsertBindings()}
  ${3:view.renderWithTemplate(view)}
  ${4:}
  return view
}
]]></content>
  <tabTrigger>render</tabTrigger>
  <scope>source.js, source.jsx, source.ts</scope>
  <description>render function</description>
</snippet>
```

### [renderCollection](https://ampersandjs.com/docs/#ampersand-view-rendercollection) function

**Trigger:** renderCollection

```xml
<snippet>
  <content><![CDATA[
view.renderCollection(${1:collection}, ${2:ItemView}, ${3:containerEl}${4:, ${5:viewOptions}})
]]></content>
  <tabTrigger>renderCollection</tabTrigger>
  <scope>source.js, source.jsx, source.ts</scope>
  <description>renderCollection function</description>
</snippet>
```

### [renderSubview](https://ampersandjs.com/docs/#ampersand-view-rendersubview) function

**Trigger:** renderSubview

```xml
<snippet>
  <content><![CDATA[
view.renderSubview(${1:viewInstance}, ${2:containerEl})
]]></content>
  <tabTrigger>renderSubview</tabTrigger>
  <scope>source.js, source.jsx, source.ts</scope>
  <description>renderSubview function</description>
</snippet>
```

### [renderWithTemplate](https://ampersandjs.com/docs/#ampersand-view-renderwithtemplate) function

**Trigger:** renderWithTemplate

```xml
<snippet>
  <content><![CDATA[
view.renderWithTemplate(${1:view}, ${2:view.template})
]]></content>
  <tabTrigger>renderWithTemplate</tabTrigger>
  <scope>source.js, source.jsx, source.ts</scope>
  <description>renderWithTemplate function</description>
</snippet>
```