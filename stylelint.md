## stylelint的最基本配置

我们使用stylelint要完成最基本的css检测配置，如下

### 安装

pnpm add postcss postcss-html stylelint  stylelint-config-standard stylelint-config-standard-vue stylelint-order

### 配置文件（.stylelintrc.json）

{

  "extends": [

   "stylelint-config-standard",

   "stylelint-config-standard-vue"

  ],

  "plugins": ["stylelint-order"],

  "overrides": [

   {

​    "files": ["**/*.(html|vue)"],

​    "customSyntax": "postcss-html"

   }

  ],

  "ignoreFiles": [

   "**/*.js",

   "**/*.jsx",

   "**/*.tsx",

   "**/*.ts",

   "**/*.json",

   "**/*.md",

   "**/*.yaml"

  ],

  "rules": {

   "no-descending-specificity": null, 

   "selector-pseudo-element-no-unknown": [

​    true,

​    {

​     "ignorePseudoElements": ["v-deep"]

​    }

   ],

   "selector-pseudo-class-no-unknown": [

​    true,

​    {

​     "ignorePseudoClasses": ["deep"]

​    }

   ],



   "order/properties-order": [

​    "position",

​    "top",

​    "right",

​    "bottom",

​    "left",

​    "z-index",

​    "display",

​    "justify-content",

​    "align-items",

​    "float",

​    "clear",

​    "overflow",

​    "overflow-x",

​    "overflow-y",

​    "padding",

​    "padding-top",

​    "padding-right",

​    "padding-bottom",

​    "padding-left",

​    "margin",

​    "margin-top",

​    "margin-right",

​    "margin-bottom",

​    "margin-left",

​    "width",

​    "min-width",

​    "max-width",

​    "height",

​    "min-height",

​    "max-height",

​    "font-size",

​    "font-family",

​    "text-align",

​    "text-justify",

​    "text-indent",

​    "text-overflow",

​    "text-decoration",

​    "white-space",

​    "color",

​    "background",

​    "background-position",

​    "background-repeat",

​    "background-size",

​    "background-color",

​    "background-clip",

​    "border",

​    "border-style",

​    "border-width",

​    "border-color",

​    "border-top-style",

​    "border-top-width",

​    "border-top-color",

​    "border-right-style",

​    "border-right-width",

​    "border-right-color",

​    "border-bottom-style",

​    "border-bottom-width",

​    "border-bottom-color",

​    "border-left-style",

​    "border-left-width",

​    "border-left-color",

​    "border-radius",

​    "opacity",

​    "filter",

​    "list-style",

​    "outline",

​    "visibility",

​    "box-shadow",

​    "text-shadow",

​    "resize",

​    "transition"

   ]

  }

 }

## stylelint与sass的基本配置

### 安装

pnpm add postcss postcss-html stylelint  stylelint-config-standard stylelint-config-standard-vue stylelint-order  stylelint-config-recommended-scss stylelint-config-recess-order stylelint-config-standard-scss postcss-scss

### 配置文件（.stylelintrc.json）

{

  "extends": [

   "stylelint-config-standard",

   "stylelint-config-standard-vue",

   "stylelint-config-recommended-vue/scss",

   "stylelint-config-standard-scss",

   "stylelint-config-recess-order"

  ],

  "plugins": ["stylelint-order"],

  "overrides": [

   {

​    "files":["**/*.(scss|css|vue|html)"], 

​    "customSyntax": "postcss-scss"

   },

   {

​    "files": ["**/*.(html|vue)"],

​    "customSyntax": "postcss-html"

   }

  ],

  "ignoreFiles": [

   "**/*.js",

   "**/*.jsx",

   "**/*.tsx",

   "**/*.ts",

   "**/*.json",

   "**/*.md",

   "**/*.yaml"

  ],

  "rules": {

   "no-descending-specificity": null, 

   "selector-pseudo-element-no-unknown": [

​    true,

​    {

​     "ignorePseudoElements": ["v-deep"]

​    }

   ],

   "selector-pseudo-class-no-unknown": [

​    true,

​    {

​     "ignorePseudoClasses": ["deep"]

​    }

   ],



   "order/properties-order": [

​    "position",

​    "top",

​    "right",

​    "bottom",

​    "left",

​    "z-index",

​    "display",

​    "justify-content",

​    "align-items",

​    "float",

​    "clear",

​    "overflow",

​    "overflow-x",

​    "overflow-y",

​    "padding",

​    "padding-top",

​    "padding-right",

​    "padding-bottom",

​    "padding-left",

​    "margin",

​    "margin-top",

​    "margin-right",

​    "margin-bottom",

​    "margin-left",

​    "width",

​    "min-width",

​    "max-width",

​    "height",

​    "min-height",

​    "max-height",

​    "font-size",

​    "font-family",

​    "text-align",

​    "text-justify",

​    "text-indent",

​    "text-overflow",

​    "text-decoration",

​    "white-space",

​    "color",

​    "background",

​    "background-position",

​    "background-repeat",

​    "background-size",

​    "background-color",

​    "background-clip",

​    "border",

​    "border-style",

​    "border-width",

​    "border-color",

​    "border-top-style",

​    "border-top-width",

​    "border-top-color",

​    "border-right-style",

​    "border-right-width",

​    "border-right-color",

​    "border-bottom-style",

​    "border-bottom-width",

​    "border-bottom-color",

​    "border-left-style",

​    "border-left-width",

​    "border-left-color",

​    "border-radius",

​    "opacity",

​    "filter",

​    "list-style",

​    "outline",

​    "visibility",

​    "box-shadow",

​    "text-shadow",

​    "resize",

​    "transition"

   ]

  }

 }

## stylelint与less的基本配置

### 安装

pnpm add postcss postcss-html stylelint  stylelint-config-standard stylelint-config-standard-vue stylelint-order postcss-less stylelint-config-recommended-less

### 配置文件（.stylelintrc.json）

{

  "extends": [

   "stylelint-config-standard",

   "stylelint-config-standard-vue",

   "stylelint-config-recommended-less",

   "stylelint-config-recess-order"

  ],

  "plugins": ["stylelint-order"],

  "overrides": [

   {

​    "files":["**/*.(less|css|vue|html)"], 

​    "customSyntax": "postcss-less"

   },

   {

​    "files": ["**/*.(html|vue)"],

​    "customSyntax": "postcss-html"

   }

  ],

  "ignoreFiles": [

   "**/*.js",

   "**/*.jsx",

   "**/*.tsx",

   "**/*.ts",

   "**/*.json",

   "**/*.md",

   "**/*.yaml"

  ],

  "rules": {

   "no-descending-specificity": null, 

   "selector-pseudo-element-no-unknown": [

​    true,

​    {

​     "ignorePseudoElements": ["v-deep"]

​    }

   ],

   "selector-pseudo-class-no-unknown": [

​    true,

​    {

​     "ignorePseudoClasses": ["deep"]

​    }

   ],



   "order/properties-order": [

​    "position",

​    "top",

​    "right",

​    "bottom",

​    "left",

​    "z-index",

​    "display",

​    "justify-content",

​    "align-items",

​    "float",

​    "clear",

​    "overflow",

​    "overflow-x",

​    "overflow-y",

​    "padding",

​    "padding-top",

​    "padding-right",

​    "padding-bottom",

​    "padding-left",

​    "margin",

​    "margin-top",

​    "margin-right",

​    "margin-bottom",

​    "margin-left",

​    "width",

​    "min-width",

​    "max-width",

​    "height",

​    "min-height",

​    "max-height",

​    "font-size",

​    "font-family",

​    "text-align",

​    "text-justify",

​    "text-indent",

​    "text-overflow",

​    "text-decoration",

​    "white-space",

​    "color",

​    "background",

​    "background-position",

​    "background-repeat",

​    "background-size",

​    "background-color",

​    "background-clip",

​    "border",

​    "border-style",

​    "border-width",

​    "border-color",

​    "border-top-style",

​    "border-top-width",

​    "border-top-color",

​    "border-right-style",

​    "border-right-width",

​    "border-right-color",

​    "border-bottom-style",

​    "border-bottom-width",

​    "border-bottom-color",

​    "border-left-style",

​    "border-left-width",

​    "border-left-color",

​    "border-radius",

​    "opacity",

​    "filter",

​    "list-style",

​    "outline",

​    "visibility",

​    "box-shadow",

​    "text-shadow",

​    "resize",

​    "transition"

   ]

  }

 }