**Maintainer:** Gus Esquivel <br />
**Plugin Website:** https://github.com/gesquive/bootstrap-add-clear <br />
**Contributers:**
<a href="https://github.com/skorecky">Stephen Korecky</a>,
<a href="https://github.com/scoman81">scoman81</a>,
<a href="https://github.com/Steve887">Steve887</a>,
<a href="https://github.com/Deividy">Deividy</a>

<br />

## About
This project is a fork of Stephen Korecky's "Add Clear" project. It is meant to work as a drop-in replacement when using bootstrap.


## How to use
- Load jQuery & Bootstrap into your project
- Load Add Clear plugin into your project
- Setup which elements you would like to apply this plugin to.

### Usage
```javascript
$(function(){
  $(":input").addClear();
});
```
### Available Options

<table>
  <tr>
    <th>Option</th>
    <th>Type</th>
    <th>Default</th>
  </tr>
  <tr>
    <td>closeSymbol</td>
    <td>string</td>
    <td></td>
  </tr>
  <tr>
    <td>symbolClass</td>
    <td>string</td>
    <td>glyphicon glyphicon-remove-circle</td>
  </tr>
  <tr>
    <td>wrapperClass</td>
    <td>string</td>
    <td></td>
  </tr>
  <tr>
    <td>top</td>
    <td>number</td>
    <td>0</td>
  </tr>
  <tr>
    <td>right</td>
    <td>number</td>
    <td>0</td>
  </tr>
  <tr>
    <td>returnFocus</td>
    <td>boolean</td>
    <td>true</td>
  </tr>
  <tr>
    <td>showOnLoad</td>
    <td>boolean</td>
    <td>false</td>
  </tr>
  <tr>
    <td>clearOnEscape</td>
    <td>boolean</td>
    <td>true</td>
  </tr>
  <tr>
    <td>hideOnBlur</td>
    <td>boolean</td>
    <td>false</td>
  </tr>
  <tr>
    <td>onClear</td>
    <td>function</td>
    <td>null</td>
  </tr>
</table>

#### Using Options
```javascript
$("input").addClear({top : -2, right : 6});

// Example onClear option usage
$(":input").addClear({
  onClear: function(){
    alert("call back!");
  }
});

// Example font awesome icon usage
$(":input").addClear({
    symbolClass: "fa fa-times-circle"
})
```
