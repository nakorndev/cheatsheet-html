# HTML Cheatsheet

รวมสูตรโกงสำหรับการใช้งาน HTML

## 📝 โปรแกรมแก้ไขโค้ด

- [ติดตั้ง VSCode](https://code.visualstudio.com/)
- [ส่วนเสริม Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
- [ส่วนเสริม W3C Validation](https://marketplace.visualstudio.com/items?itemName=Umoxfo.vscode-w3cvalidation)
- [Java 8 สำหรับใช้ W3C Validation](https://www.oracle.com/java/technologies/javase-jre8-downloads.html)

## 👍 เว็บไซต์รวบรวมการใช้ HTML

- [https://htmlreference.io/](https://htmlreference.io/)
- [https://www.w3schools.com/html/default.asp](https://www.w3schools.com/html/default.asp)
- [https://developer.mozilla.org/en-US/docs/Web/HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)

## 🏗️ โครงสร้างภาพรวม

```html
<!-- normal tag -->
<div class="title">Hello!</div>
  ⬇    ⬇     ⬇       ⬇      ⬇
  ⬇    ⬇     ⬇       ⬇      ⬇
  ⬇    ⬇     ⬇      content ⬇
  ⬇    ⬇     ⬇              ⬇
  ⬇    ⬇  attribute value   ⬇
  ⬇    ⬇                    ⬇
  ⬇  attribute name        close tag
  ⬇
 open tag

<!-- self-closing tag -->
<img src="icon/logo.png" alt="Logo">
```

## 🔲 การแสดงผลแบบ Inline และ Block

![inline-and-block](https://i.imgur.com/VLM9RRj.png)

```html
<!-- ทั้งหมดจะไม่มี Style ใดๆ เช่น ข้อความใหญ่ ข้อความตัวหนา -->
<span>Inline</span>
<span>Inline</span>
<span>Inline</span>
<div>Block</div>
<div>Block</div>
<div>Block</div>
```

## 📚 Semantic Tags

![semantic-layout](https://i.imgur.com/vCaSxAS.png)

```html
<nav>แถบนำทาง</nav>
<header>ส่วนหัว</header>
<article>บทความ</article>
<aside>ด้านข้างซ้ายหรือขวา</aside>
<main>เนื้อหาหลัก</main>
<section>ส่วนประกอบทั่วไป</section>
<footer>ส่วนล่าง</footer>
```

## 💬 Comment Tag

```html
<!-- Comment me! -->
```

> บน VSCode สามารถกดปุ่ม `Ctrl + /` หรือ `Ctrl + ฝ` เพื่อสร้าง Comment tag อย่างรวดเร็วได้

## 📌 กำหนด Title และ Favicon

![title-and-favicon](https://i.imgur.com/Ja2oTBC.jpg)

```html
<head>
  <title>Change me!</title>

  <!-- Snippet: link:favicon -->
  <link rel="shortcut icon" href="path/of/favicon.ico" type="image/x-icon">

  <!-- ไฟล์นามสกุล .png (ไม่แนะนำ) -->
  <link rel="shortcut icon" href="path/of/favicon.png" type="image/png">
</head>
```

## 🔣 Entities Code

|Code|Symbol|
|-|-|
|`&nbsp;`|(เว้นวรรค)|
|`&lt;`|&lt;|
|`&gt;`|&gt;|
|`&larr;`|&larr;|
|`&uarr;`|&uarr;|
|`&rarr;`|&rarr;|
|`&darr;`|&darr;|
|`&dollar;`|&dollar;|
|`&cent;`|&cent;|
|`&pound;`|&pound;|
|`&euro;`|&euro;|
|`&yen;`|&yen;|
|`&copy;`|&copy;|
|`&reg;`|&reg;|
|`&trade;`|&trade;|
|`&para;`|&para;|
|`&micro;`|&micro;|
|`&horbar;`|&horbar;|
|`&nldr;`|&nldr;|
|`&hellip;`|&hellip;|
|`&plus;`|&plus;|
|`&minus;`|&minus;|
|`&times;`|&times;|
|`&divide;`|&divide;|
|`&equals;`|&equals;|
|`&ne;`|&ne;|
|`&female;`|&female;|
|`&male;`|&male;|
|`&check;`|&check;|
|`&#10005;`|&#10005;|
|`&#9745;`|&#9745;|
|`&#9746;`|&#9746;|
|`&#8451;`|&#8451;|
|`&#8457;`|&#8457;|
|`&#9888;`|&#9888;|
|`&#9993;`|&#9993;|

> ดูเพิ่มเติมที่ [toptal.com](https://www.toptal.com/designers/htmlarrows/symbols/)

## 🔤 Text Formatting

```html
<!-- Block -->
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
<p>Paragraph</p>
<blockquote>Blockquote</blockquote>

<!-- Inline -->
<b>Bold</b>
<i>Italic</i>
<u>Underline</u>
<s>Strikethrough</s>
<sup>Superscript</sup>
<sub>Subscript</sub>
<code>Code</code>
<var>Variable</var>
<kbd>Keyboard definition</kbd>
<samp>Sample output</samp>
<abbr title="Abbr">Abbreviation</abbr>

<!-- Line -->
<br> <!-- Break line -->
<hr> <!-- Horizontal line -->
```

## 📃 List

```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>

<ul>
  <li>
    Item 1
    <ul>
      <li>Item 1.1</li>
      <li>Item 1.2</li>
      <li>Item 1.3</li>
    </ul>
  </li>
</ul>

<ol type="A" start="10">
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ol>
```

## 🔗 Link (Anchor)

```html
<a href="https://www.google.com">Google</a>
<a href="https://www.google.com" target="_blank">Google (New tab)</a>
<a href="index.html">index.html</a>
<a href="tel:027777777">SCB Telephone</a>
<a href="mailto:nakorndev@gmail.com">Mail to mentor</a>

<!-- Document fragment -->
<a href="#top">Go to top (top of page)</a>
<a href="#apple">Go to apple (math with id)</a>
<h1 id="apple">Apple</h1>
```

## 🛣️ การกำหนด Path (เส้นทางที่อยู่ข้อมูล)

|Keywords|การทำงาน|Code|
|-|-|-|
|Root|ตำแหน่งรากฐาน|`/index.html`|
|Current|ตำแหน่งที่อยู่ปัจจุบัน|`index.html` หรือ `./index.html`|
|Parent|ตำแหน่งที่อยู่ก่อนหน้า|`../index.html`|

## 📷 Media

```html
<!-- Image -->
<img src="http://via.placeholder.com/150" alt="Generate by Placeholder.com">

<!-- Link as image -->
<a href="to/new/url">
  <img src="path/to/image.png" alt="name of image">
</a>

<!-- Image with caption -->
<figure>
  <img src="path/to/image.jpg" alt="My Image">
  <figcaption>My Image</figcaption>
</figure>

<!-- Video -->
<video src="path/of/video" controls>Web browser not support</video>

<!-- Video (Multiple file supports) -->
<video>
  <source src="path/video.mp4" type="video/mp4">
  <source src="path/video.ogg" type="video/ogg">
  Web browser not support
</video>

<!-- Audio -->
<video src="path/of/audio" controls>Web browser not support</video>

<!-- Iframe -->
<iframe src="http://example.com" width="400" height="250"></iframe>

<!-- Embed (YouTube) -->
<iframe width="1280" height="720" src="https://www.youtube.com/embed/UZnIHM2dQvA" title="YouTube video player" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
```

## 📊 Table

```html
<table>
  <!-- Table name -->
  <caption>My Table</caption>

  <!-- Head -->
  <thead>
    <tr>
      <th>Title 1</th>
      <th>Title 2</th>
    </tr>
  </thead>

  <!-- Body -->
  <tbody>
    <tr>
      <td>Item 1</td>
      <td>Item 2</td>
    </tr>
    <tr>
      <td colspan="2">Item 3-4</td>
    </tr>
    <tr>
      <td rowspan="2">Item 6</td>
      <td>Item 7</td>
    </tr>
    <tr>
      <td>Item 8</td>
    </tr>
  </tbody>

  <!-- Foot -->
  <tfoot>
    <tr>
      <th>Foot 1</th>
      <th>Foot 2</th>
    </tr>
  </tfoot>
</table>
```

## ⌨️ Form

```html
<!-- Form -->
<form action="path/to/submit" method="POST">
  <input name="username" type="text">
  <input name="password" type="text">
  <button>Submit</button>
</form>

<!-- Label -->
<label for="username">Username:</label>
<input id="username" type="text">

<label>
  Username:
  <input type="text">
</label>
```

## ⌨️ Form types & attributes

```html
<!-- All types -->
<input type="text">     <!-- ข้อความ -->
<input type="password"> <!-- รหัสผ่าน -->
<input type="email">    <!-- อีเมล -->
<input type="tel">      <!-- โทรศัพท์ -->
<input type="url">      <!-- ลิงก์ -->
<input type="search">   <!-- ค้นหา -->
<input type="number">   <!-- จำนวน -->
<input type="range">    <!-- ขนาด -->
<input type="color">    <!-- สี -->
<input type="time">     <!-- เวลา -->
<input type="date">     <!-- วันที่ -->
<input type="week">     <!-- สัปดาห์ -->
<input type="month">    <!-- เดือน -->
<input type="datetime-local"> <!-- วันและเวลา -->
<input type="checkbox"> <!-- ทำเครื่องหมาย -->
<input type="radio">    <!-- ทางเลือก -->
<input type="file">     <!-- ไฟล์ -->
<input type="hidden">   <!-- ซ่อน -->

<!-- All attributes -->
<input type="text" value="Hello!">      <!-- ค่าเริ่มต้น -->
<input type="text" name="username">     <!-- ชื่อฟิลด์ -->
<input type="text" placeholder="Please input me"> <!-- แสดงเมื่อไม่ใส่ค่า -->
<input type="text" required>            <!-- ต้องมีค่าถึงจะดำเนินการต่อได้ -->
<input type="text" readonly>            <!-- อ่านได้อย่างเดียว -->
<input type="text" disabled>            <!-- ปิดใช้งาน และส่งข้อมูลไม่ได้ -->
<input type="text" autocomplete="off">  <!-- ปิดใช้งาน Autocomplete -->
<input type="text" autofocus>           <!-- เริ่มโฟกัสพร้อมพิมพ์ได้ทันที -->
<input type="text" tabindex="-1">       <!-- กำหนดลำดับความสำคัญของ Tab (ค่าเริ่มต้น: 0, ปิดใช้งาน: -1) -->
<input type="checkbox" checked>         <!-- ทำเครื่องหมายเป็นค่าเริ่มต้น -->
<input type="text" minlength="3">       <!-- ต้องการข้อมูลอย่างน้อย 3 ตัวอักษร -->
<input type="text" maxlength="12">      <!-- ต้องการข้อมูลมากสุด 12 ตัวอักษร -->
<input type="number" min="18">          <!-- ต้องการตัวเลขอย่างน้อย 18 -->
<input type="number" max="30">          <!-- ต้องการตัวเลขได้มากสุด 30 -->
<input type="number" step="5">          <!-- เพิ่มและลดค่าทีล่ะ 5 หน่วย -->
<input type="file" accept="image/*">    <!-- เลือกไฟล์ได้เฉพาะรูปภาพ -->
<input type="file" accept=".jpg">       <!-- เลือกไฟล์ได้เฉพาะนามสกุลไฟล์ .jpg -->
<input type="file" multiple>            <!-- เลือกได้หลายไฟล์ -->

<!-- Radio -->
<label>
  Male: <input name="gender" type="radio" value="male">
</label>

<label>
  Female: <input name="gender" type="radio" value="female">
</label>

<label>
  None: <input name="gender" type="radio" value="none">
</label>
```

## ⌨️ Other form

```html
<!-- Textarea -->

<textarea name="body" cols="30" rows="10">Hello world!</textarea>

<!-- Select -->

<select name="fruits">
  <option value="apple">Apple</option>
  <option value="banana" selected>Banana</option>
  <option value="cherry">Cherry</option>
</select>

<select>
  <optgroup label="Languages">
    <option value="th">Thai</option>
    <option value="en">English</option>
  </optgroup>
  <optgroup label="Country">
    <option value="thai">Thailand</option>
    <option value="usa">United State</option>
  </optgroup>
</select>

<!-- Datalist -->

<datalist id="province">
  <option value="bkk">กรุงเทพฯ</option>
  <option value="phm">ปทุมธานี</option>
  <option value="ntb">นนทบุรี</option>
</datalist>

<input list="province" type="text">

<!-- Buttons -->
<button>Submit</button> <!-- type="submit" by default -->
<button type="button">Button</button>
<button type="reset">Reset</button>
```
