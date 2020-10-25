# React Color Selector

## **Description:** 
**react-color-selector** is a very useful and easy to use color picker, no external dependency is needed for this. You can chagne theme of it's color, by simply editing css variables. One of the best featur is you can use *any number of columns and rows for your color palette.*

### **How to install?**
```
npm i react-color-selector
```

### **Implementation**
```
import React, {useState} from 'react';
import ColorSelector from 'react-color-selector';


const App = () => {
    let [myColor, pickedColor] = useState('');
    let picker_data = {
        col: 12,
        row: 12,
        width: 300,
        height: 250,
        view: 'both', 
        theme: 'dark'
    }
    return (
        ....
        <ColorSelector pallet={picker_data} selectedColor={pickedColor} />
        <p>{myColor}</>
    )
}
export default App;
```


**react-color-selector** returns a string value of hex color code like **#4d0026**, in this above code, **myColor** will have the returned hex color code

*Color Selector doesn't come with any pre-defined button, so you can open or close this component on a freedom of your own button click function*




## **Theming:** 
**react-color-selector** comes with two themes, light and dark. In your **picker_data** object select **theme** and set value either **dark** or **light**. By default it is **light**.

There is small css theme is needed. These **primary** theme concept is provided for branding purpose. It will take your projects primary color, if it has, otherwise *provide a root variable for primary color*

```
:root {
  --primary: #007bff;
}
```
## **Options**
| Properties  | Type | Description | Example |
| ------------- | ------------- | ------------- |------------- |
| **col**  | **Number**  | *Provides number of column in color pallate* | **col:12**|
| **row**  | **Number**  | *Creates number or rows in color pallate* | **row:12**|
| **width**  | **Number**  | *Width of the color pallate canvas* | **width:300**|
| **height**  | **Number**  | *Height of the color pallate canvas* | **width:250**|
| **view**  | **string**  | ***palette** and **sphere** or you can use **both*** | **view:'both'**|
| **theme**  | **string**  | ***dark** or **light** by default its light* | **theme:'dark'**|

--------------------------------------------



## **Raise an Issue**
If you are facing any issue regarding installation and usage, raise your issue in **Git repo**. 
```
https://github.com/devsubhajit/react-color-selector/issues
```
