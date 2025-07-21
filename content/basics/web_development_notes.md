---
title: Web Development Notes
date: 2025-07-21
author: Your Name
cell_count: 18
score: 15
---

<style>
  .card {
    width: 350px;
    padding: 20px;
    background: #f0f8ff;
    border: 2px solid #4b9cd3;
    border-radius: 15px;
    font-family: 'Segoe UI', sans-serif;
    box-shadow: 4px 4px 10px rgba(0, 0, 0, 0.1);
  }

  .card h2 {
    color: #4b9cd3;
  }

  .card p {
    color: #333;
    line-height: 1.5;
  }

  .btn {
    background-color: #4b9cd3;
    color: white;
    padding: 10px 20px;
    border: none;
    border-radius: 8px;
    text-decoration: none;
    display: inline-block;
    margin-top: 10px;
    cursor: pointer;
  }

  .btn:hover {
    background-color: #357ca5;
  }
</style>

<div class="card">
  <h2>Welcome to My Web Component</h2>
  <p>This is an embedded HTML + CSS card inside a Jupyter Notebook. You can style it however you like!</p>
  <a href="https://github.com/" target="_blank" class="btn">Visit GitHub</a>
</div>




<!-- Inline and Block Elements Demo -->

<span style="border: 2px solid red;">This is a span element</span>
<em style="border: 2px solid blue;">This is an emphasized text</em>

<br><br>

<span style="border: 2px solid blue;">This is another span</span>
<span style="border: 2px solid orangered;">This is also a span</span>
 


```python

```

<style>
  body {
    margin: 0;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #000;
  }

  .container {
    text-align: center;
  }

  .box {
    font-family: 'Anton', sans-serif;
    font-size: 100px;
    color: white;
    letter-spacing: 8px;
  }

  .footer, .starting, .engine, .rights, .unreal, .lnc {
    color: #888;
    font-family: Arial, sans-serif;
    margin-top: 10px;
    font-size: 14px;
  }

  .starting {
    font-size: 24px;
    color: white;
  }

  .start-button {
    margin-top: 30px;
    padding: 10px 20px;
    font-size: 16px;
    background-color: #28a745;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
  }

  .start-button:hover {
    background-color: #218838;
  }
</style>

<div class="container">
  <div class="box">KRAFTON</div>
  <div class="footer">© 2017 KRAFTON, Inc. All rights reserved.</div>
  <div class="starting">Starting...</div>
  <div class="engine">Unreal Engine, Copyright 1998-2025, Epic Games, Inc.</div>
  <div class="rights">All rights reserved</div>
  <div class="unreal">Unreal is a trademark or registered trademark of Epic Games.</div>
  <div class="lnc">Inc. in the United States of America and elsewhere</div>
  <button class="start-button">Start</button>
</div>


<style>
  .login-container {
    background-color: white;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    width: 300px;
    margin: 100px auto;
    font-family: Arial, sans-serif;
  }

  h2 {
    text-align: center;
    color: #333;
  }

  .input-field {
    width: 100%;
    padding: 10px;
    margin: 10px 0;
    border: 1px solid #ccc;
    border-radius: 5px;
  }

  .btn {
    width: 100%;
    padding: 10px;
    background-color: #28a745;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-size: 16px;
  }

  .btn:hover {



```python
from IPython.display import display, HTML

signup_html = """
<style>
  body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background: url('images/kraft1.jpg') no-repeat center center fixed;
    background-size: cover;
  }

  .signup-container {
    background-color: white;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    width: 300px;
  }

  h2 {
    text-align: center;
    color: #333;
  }

  .input-field {
    width: 100%;
    padding: 10px;
    margin: 10px 0;
    border: 1px solid #ccc;
    border-radius: 5px;
  }

  .btn {
    width: 100%;
    padding: 10px;
    background-color: #28a745;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-size: 16px;
  }

  .btn:hover {
    background-color: #218838;
  }

  .login-link {
    text-align: center;
    margin-top: 10px;
  }

  .login-link a {
    color: #007bff;
    text-decoration: none;
  }
</style>

<div class="signup-container">
  <h2>Signup</h2>
  <form>
    <input type="text" class="input-field" name="username" placeholder="Username" required />
    <input type="email" class="input-field" name="email" placeholder="Email" required />
    <input type="password" class="input-field" name="password" placeholder="Password" required />
    <input type="password" class="input-field" name="confirm_password" placeholder="Confirm Password" required />
    <button type="submit" class="btn">Sign Up</button>
  </form>
  <div class="login-link">
    <p>Already have an account? <a href="#">Login here</a></p>
  </div>
</div>
"""

display(HTML(signup_html))

```



<style>
  body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background: url('images/kraft1.jpg') no-repeat center center fixed;
    background-size: cover;
  }

  .signup-container {
    background-color: white;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    width: 300px;
  }

  h2 {
    text-align: center;
    color: #333;
  }

  .input-field {
    width: 100%;
    padding: 10px;
    margin: 10px 0;
    border: 1px solid #ccc;
    border-radius: 5px;
  }

  .btn {
    width: 100%;
    padding: 10px;
    background-color: #28a745;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-size: 16px;
  }

  .btn:hover {
    background-color: #218838;
  }

  .login-link {
    text-align: center;
    margin-top: 10px;
  }

  .login-link a {
    color: #007bff;
    text-decoration: none;
  }
</style>

<div class="signup-container">
  <h2>Signup</h2>
  <form>
    <input type="text" class="input-field" name="username" placeholder="Username" required />
    <input type="email" class="input-field" name="email" placeholder="Email" required />
    <input type="password" class="input-field" name="password" placeholder="Password" required />
    <input type="password" class="input-field" name="confirm_password" placeholder="Confirm Password" required />
    <button type="submit" class="btn">Sign Up</button>
  </form>
  <div class="login-link">
    <p>Already have an account? <a href="#">Login here</a></p>
  </div>
</div>







from IPython.display import display, HTML

login_html = """
<style>
  body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
  }

  .login-container {
    background-color: white;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    width: 300px;
  }

  h2 {
    text-align: center;
    color: #333;
  }

  .input-field {
    width: 100%;
    padding: 10px;
    margin: 10px 0;
    border: 1px solid #ccc;
    border-radius: 5px;
  }

  .btn {
    width: 100%;
    padding: 10px;
    background-color: #28a745;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    font-size: 16px;
  }

  .btn:hover {
    background-color: #218838;
  }

  .signup-link {
    text-align: center;
    margin-top: 10px;
  }

  .signup-link a {
    color: #007bff;
    text-decoration: none;
  }
</style>

<div class="login-container">
  <h2>Login</h2>
  <form>
    <input type="email" class="input-field" name="email" placeholder="Email" required />
    <input type="password" class="input-field" name="password" placeholder="Password" required />
    <button type="submit" class="btn">Login</button>
  </form>
  <div class="signup-link">
    <p>Don't have an account? <a href="#">Sign up here</a></p>
  </div>
</div>
"""

display(HTML(login_html))



```python
from IPython.core.display import display, HTML

display(HTML("<h1>Main Heading (h1)</h1><p>This is a paragraph.</p>"))


```

    C:\Users\sahil\AppData\Local\Temp\ipykernel_10400\3068744958.py:1: DeprecationWarning: Importing display from IPython.core.display is deprecated since IPython 7.14, please import from IPython.display
      from IPython.core.display import display, HTML
    


<h1>Main Heading (h1)</h1><p>This is a paragraph.</p>



```python
from IPython.core.display import display, HTML

form_html = """
<form action="/login" method="post">
  <label for="username">Username:</label><br>
  <input type="text" id="username" name="username"><br>

  <label for="password">Password:</label><br>
  <input type="password" id="password" name="password"><br><br>

  <input type="submit" value="Login">
</form>
"""

display(HTML(form_html))

```

    C:\Users\sahil\AppData\Local\Temp\ipykernel_10400\3996564675.py:1: DeprecationWarning: Importing display from IPython.core.display is deprecated since IPython 7.14, please import from IPython.display
      from IPython.core.display import display, HTML
    



<form action="/login" method="post">
  <label for="username">Username:</label><br>
  <input type="text" id="username" name="username"><br>

  <label for="password">Password:</label><br>
  <input type="password" id="password" name="password"><br><br>

  <input type="submit" value="Login">
</form>




```python
from IPython.core.display import display, HTML

table_html = """
<table border="1" cellpadding="8" cellspacing="0">
  <tr>
    <th>Name</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Sahil</td>
    <td>22</td>
  </tr>
</table>
"""

display(HTML(table_html))

```

    C:\Users\sahil\AppData\Local\Temp\ipykernel_10400\3502825968.py:1: DeprecationWarning: Importing display from IPython.core.display is deprecated since IPython 7.14, please import from IPython.display
      from IPython.core.display import display, HTML
    



<table border="1" cellpadding="8" cellspacing="0">
  <tr>
    <th>Name</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Sahil</td>
    <td>22</td>
  </tr>
</table>




```python
from IPython.core.display import display, HTML

link_img_html = """
<a href="https://www.google.com" target="_blank">Visit Google</a>
<br><br>
<img src="https://via.placeholder.com/150" alt="Placeholder Image">
"""

display(HTML(link_img_html))

```

    C:\Users\sahil\AppData\Local\Temp\ipykernel_10400\2356580883.py:1: DeprecationWarning: Importing display from IPython.core.display is deprecated since IPython 7.14, please import from IPython.display
      from IPython.core.display import display, HTML
    



<a href="https://www.google.com" target="_blank">Visit Google</a>
<br><br>
<img src="https://via.placeholder.com/150" alt="Placeholder Image">




```python
from IPython.core.display import display, HTML

video_html = """
<iframe width="300" height="200"
  src="https://www.youtube.com/embed/dQw4w9WgXcQ"
  frameborder="0"
  allowfullscreen>
</iframe>
"""

display(HTML(video_html))

```

    C:\Users\sahil\AppData\Local\Temp\ipykernel_10400\890135510.py:1: DeprecationWarning: Importing display from IPython.core.display is deprecated since IPython 7.14, please import from IPython.display
      from IPython.core.display import display, HTML
    



<iframe width="300" height="200"
  src="https://www.youtube.com/embed/dQw4w9WgXcQ"
  frameborder="0"
  allowfullscreen>
</iframe>




```python
from IPython.core.display import display, HTML

list_html = """
<h3>Unordered List</h3>
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>

<h3>Ordered List</h3>
<ol>
  <li>Login</li>
  <li>Dashboard</li>
  <li>Logout</li>
</ol>
"""

display(HTML(list_html))

```

    C:\Users\sahil\AppData\Local\Temp\ipykernel_10400\2929690291.py:1: DeprecationWarning: Importing display from IPython.core.display is deprecated since IPython 7.14, please import from IPython.display
      from IPython.core.display import display, HTML
    



<h3>Unordered List</h3>
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>

<h3>Ordered List</h3>
<ol>
  <li>Login</li>
  <li>Dashboard</li>
  <li>Logout</li>
</ol>




```python

```


```python

```


---
**Score: 15**