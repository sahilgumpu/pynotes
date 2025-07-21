---
title: Web Development Notes
date: 2025-07-21
author: Your Name
cell_count: 45
score: 45
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
from IPython.core.display import display, HTML

css_tutorial_html = """
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Tutorial</title>
    <style>
        p {
            color: purple;
            background-color: green;
            padding: 10px;
            font-family: Arial, sans-serif;
        }
        h1 {
            color: blue;
            font-size: 24px;
        }
    </style>
</head>
<body>
    <h1>This is a CSS Tutorial</h1>
    <!-- <p style="color: red;background-color: yellow;">This tutorial will teach you everything you need to know about HTML/CSS</p> -->
    <p>This tutorial will teach you everything you need to know about HTML/CSS</p>
</body>
</html>
"""

display(HTML(css_tutorial_html))

```

    C:\Users\sahil\AppData\Local\Temp\ipykernel_2864\551637126.py:1: DeprecationWarning: Importing display from IPython.core.display is deprecated since IPython 7.14, please import from IPython.display
      from IPython.core.display import display, HTML
    



<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Tutorial</title>
    <style>
        p {
            color: purple;
            background-color: green;
            padding: 10px;
            font-family: Arial, sans-serif;
        }
        h1 {
            color: blue;
            font-size: 24px;
        }
    </style>
</head>
<body>
    <h1>This is a CSS Tutorial</h1>
    <!-- <p style="color: red;background-color: yellow;">This tutorial will teach you everything you need to know about HTML/CSS</p> -->
    <p>This tutorial will teach you everything you need to know about HTML/CSS</p>
</body>
</html>




```python
from IPython.core.display import display, HTML

css_selectors_html = """
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Selectors</title>
    <style>
        p {
            border: 2px solid rebeccapurple;
            padding: 5px;
        }
        /* Id selector */
        #firstpara {
            color: red;
        }
        /* Class selector */
        .bgBlue {
            color: green;
            background-color: black;
        }
        /* Multiple element selector */
        footer, span {
            background-color: pink;
            padding: 5px;
            display: inline-block;
            margin-top: 5px;
        }
    </style>
</head>
<body>
    <h3>CSS Selectors</h3>
    <p id="firstpara">This is a simple paragraph to demonstrate CSS selectors</p>
    <p id="secondPara" class="bgBlue">This is another paragraph with class "bgBlue"</p>
    <div>
        <p>This is yet another paragraph inside a div</p>
        <span>This is a span element</span>
        <footer>This is a footer element</footer>
    </div>
</body>
</html>
"""

display(HTML(css_selectors_html))

```

    C:\Users\sahil\AppData\Local\Temp\ipykernel_2864\3174135209.py:1: DeprecationWarning: Importing display from IPython.core.display is deprecated since IPython 7.14, please import from IPython.display
      from IPython.core.display import display, HTML
    



<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Selectors</title>
    <style>
        p {
            border: 2px solid rebeccapurple;
            padding: 5px;
        }
        /* Id selector */
        #firstpara {
            color: red;
        }
        /* Class selector */
        .bgBlue {
            color: green;
            background-color: black;
        }
        /* Multiple element selector */
        footer, span {
            background-color: pink;
            padding: 5px;
            display: inline-block;
            margin-top: 5px;
        }
    </style>
</head>
<body>
    <h3>CSS Selectors</h3>
    <p id="firstpara">This is a simple paragraph to demonstrate CSS selectors</p>
    <p id="secondPara" class="bgBlue">This is another paragraph with class "bgBlue"</p>
    <div>
        <p>This is yet another paragraph inside a div</p>
        <span>This is a span element</span>
        <footer>This is a footer element</footer>
    </div>
</body>
</html>




```python
from IPython.core.display import display, HTML

developer_tools_html = """
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Developer Tools</title>
    <style>
        p {
            color: purple;
            font-style: italic;
            background-color: rosybrown;
            padding: 10px;
            border-radius: 5px;
        }
        h1 {
            color: darkblue;
        }
    </style>
</head>
<body>
    <h1>Developer Tools Tutorial</h1>
    <p>This is a tutorial for Chrome Developer Tools</p>
</body>
</html>
"""

display(HTML(developer_tools_html))

```

    C:\Users\sahil\AppData\Local\Temp\ipykernel_2864\891464908.py:1: DeprecationWarning: Importing display from IPython.core.display is deprecated since IPython 7.14, please import from IPython.display
      from IPython.core.display import display, HTML
    



<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Developer Tools</title>
    <style>
        p {
            color: purple;
            font-style: italic;
            background-color: rosybrown;
            padding: 10px;
            border-radius: 5px;
        }
        h1 {
            color: darkblue;
        }
    </style>
</head>
<body>
    <h1>Developer Tools Tutorial</h1>
    <p>This is a tutorial for Chrome Developer Tools</p>
</body>
</html>




```python
from IPython.core.display import display, HTML

css_fonts_html = """
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Fonts</title>
    <style>
        p {
            font-family: Arial, Helvetica, sans-serif;
            font-size: 23px; /* px = 1/96th of an inch */
            line-height: 1.3em;
        }
        span {
            font-weight: bold;
            font-style: italic;
        }
        h1 {
            color: #333;
        }
    </style>
</head>
<body>
    <h1>CSS Fonts</h1>
    <p>Let's play with <span>fonts</span>. It is very exciting!</p>
</body>
</html>
"""

display(HTML(css_fonts_html))

```

    C:\Users\sahil\AppData\Local\Temp\ipykernel_2864\648337141.py:1: DeprecationWarning: Importing display from IPython.core.display is deprecated since IPython 7.14, please import from IPython.display
      from IPython.core.display import display, HTML
    



<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Fonts</title>
    <style>
        p {
            font-family: Arial, Helvetica, sans-serif;
            font-size: 23px; /* px = 1/96th of an inch */
            line-height: 1.3em;
        }
        span {
            font-weight: bold;
            font-style: italic;
        }
        h1 {
            color: #333;
        }
    </style>
</head>
<body>
    <h1>CSS Fonts</h1>
    <p>Let's play with <span>fonts</span>. It is very exciting!</p>
</body>
</html>




```python
from IPython.display import HTML, display

color_demo_html = """
<style>
    #firstPara {
        color: blueviolet;
    }
    #secondPara {
        color: rgb(223, 130, 54); /* color by RGB value */
    }
    #thirdPara {
        color: #ff88ff; /* color by HEX value */
    }
</style>

<h2>This is my first box</h2>
<p id="firstPara">This is a paragraph from the first box</p>

<h2>This is my second box</h2>
<p id="secondPara">This is a paragraph from the second box</p>

<h2>This is my third box</h2>
<p id="thirdPara">This is a paragraph from the third box</p>
"""

display(HTML(color_demo_html))

```



<style>
    #firstPara {
        color: blueviolet;
    }
    #secondPara {
        color: rgb(223, 130, 54); /* color by RGB value */
    }
    #thirdPara {
        color: #ff88ff; /* color by HEX value */
    }
</style>

<h2>This is my first box</h2>
<p id="firstPara">This is a paragraph from the first box</p>

<h2>This is my second box</h2>
<p id="secondPara">This is a paragraph from the second box</p>

<h2>This is my third box</h2>
<p id="thirdPara">This is a paragraph from the third box</p>




```python
from IPython.display import HTML

HTML("<h2 style='color: teal;'>Welcome to My Page</h2>")

```




<h2 style='color: teal;'>Welcome to My Page</h2>




```python
HTML("<p style='font-size:16px; color: gray;'>This is a styled paragraph with inline CSS.</p>")

```




<p style='font-size:16px; color: gray;'>This is a styled paragraph with inline CSS.</p>




```python
HTML("<button style='padding:10px; background: orange; color: white; border: none; border-radius: 5px;'>Click Me</button>")

```




<button style='padding:10px; background: orange; color: white; border: none; border-radius: 5px;'>Click Me</button>




```python
HTML("<span style='color:red;'>Red</span> <span style='color:green;'>Green</span> <span style='color:blue;'>Blue</span>")

```




<span style='color:red;'>Red</span> <span style='color:green;'>Green</span> <span style='color:blue;'>Blue</span>




```python
from IPython.display import HTML

HTML("""
<div style="border:1px solid #ccc; border-radius:10px; width:200px; padding:15px; text-align:center; font-family:sans-serif;">
    <img src="https://via.placeholder.com/80" style="border-radius:50%;" />
    <h3 style="margin:10px 0;">John Doe</h3>
    <p style="color:gray; font-size:14px;">Web Developer</p>
</div>
""")

```





<div style="border:1px solid #ccc; border-radius:10px; width:200px; padding:15px; text-align:center; font-family:sans-serif;">
    <img src="https://via.placeholder.com/80" style="border-radius:50%;" />
    <h3 style="margin:10px 0;">John Doe</h3>
    <p style="color:gray; font-size:14px;">Web Developer</p>
</div>





```python
HTML("""
<label for="name">Name:</label><br>
<input type="text" id="name" placeholder="Enter your name" style="padding:8px; width:200px; border:1px solid #ccc; border-radius:5px;" />
""")

```





<label for="name">Name:</label><br>
<input type="text" id="name" placeholder="Enter your name" style="padding:8px; width:200px; border:1px solid #ccc; border-radius:5px;" />





```python
HTML("""
<div style="background-color:#d1e7dd; color:#0f5132; padding:10px; border-left:5px solid #0f5132; border-radius:4px;">
    ✅ Successfully saved your data!
</div>
""")

```





<div style="background-color:#d1e7dd; color:#0f5132; padding:10px; border-left:5px solid #0f5132; border-radius:4px;">
    ✅ Successfully saved your data!
</div>





```python
HTML("""
<button style="padding:10px; border:none; border-radius:5px; background:#007bff; color:white;">📧 Email</button>
<button style="padding:10px; border:none; border-radius:5px; background:#28a745; color:white;">📞 Call</button>
""")

```





<button style="padding:10px; border:none; border-radius:5px; background:#007bff; color:white;">📧 Email</button>
<button style="padding:10px; border:none; border-radius:5px; background:#28a745; color:white;">📞 Call</button>





```python
HTML("""
<div style="font-size:24px; color:gold;">⭐ ⭐ ⭐ ⭐ ☆</div>
""")

```





<div style="font-size:24px; color:gold;">⭐ ⭐ ⭐ ⭐ ☆</div>





```python
from IPython.display import HTML

HTML("""
<div style="width:280px; margin:auto; font-family:sans-serif; padding:20px; border-radius:10px; box-shadow:0 0 10px rgba(0,0,0,0.1); background:white;">
  <h3 style="text-align:center; margin-bottom:20px;">Login</h3>
  <form>
    <input type="email" placeholder="Email" required style="width:100%; padding:10px; margin-bottom:10px; border:1px solid #ccc; border-radius:5px;" />
    <input type="password" placeholder="Password" required style="width:100%; padding:10px; margin-bottom:10px; border:1px solid #ccc; border-radius:5px;" />
    <button type="submit" style="width:100%; padding:10px; background:#28a745; color:white; border:none; border-radius:5px;">Login</button>
  </form>
</div>
""")

```





<div style="width:280px; margin:auto; font-family:sans-serif; padding:20px; border-radius:10px; box-shadow:0 0 10px rgba(0,0,0,0.1); background:white;">
  <h3 style="text-align:center; margin-bottom:20px;">Login</h3>
  <form>
    <input type="email" placeholder="Email" required style="width:100%; padding:10px; margin-bottom:10px; border:1px solid #ccc; border-radius:5px;" />
    <input type="password" placeholder="Password" required style="width:100%; padding:10px; margin-bottom:10px; border:1px solid #ccc; border-radius:5px;" />
    <button type="submit" style="width:100%; padding:10px; background:#28a745; color:white; border:none; border-radius:5px;">Login</button>
  </form>
</div>





```python
HTML("""
<div style="width:280px; margin:auto; font-family:sans-serif; padding:20px; border-radius:10px; box-shadow:0 0 10px rgba(0,0,0,0.1); background:white;">
  <h3 style="text-align:center; margin-bottom:15px;">Forgot Password</h3>
  <form>
    <input type="email" placeholder="Enter your email" required style="width:100%; padding:10px; margin-bottom:15px; border:1px solid #ccc; border-radius:5px;" />
    <button type="submit" style="width:100%; padding:10px; background:#ffc107; color:black; border:none; border-radius:5px;">Send Reset Link</button>
  </form>
</div>
""")

```





<div style="width:280px; margin:auto; font-family:sans-serif; padding:20px; border-radius:10px; box-shadow:0 0 10px rgba(0,0,0,0.1); background:white;">
  <h3 style="text-align:center; margin-bottom:15px;">Forgot Password</h3>
  <form>
    <input type="email" placeholder="Enter your email" required style="width:100%; padding:10px; margin-bottom:15px; border:1px solid #ccc; border-radius:5px;" />
    <button type="submit" style="width:100%; padding:10px; background:#ffc107; color:black; border:none; border-radius:5px;">Send Reset Link</button>
  </form>
</div>





```python
from IPython.display import HTML

HTML("""
<div style="
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  background: linear-gradient(to right, #00c6ff, #0072ff);
  font-family: Arial, sans-serif;
">
  <div style="
    background: white;
    padding: 20px;
    border-radius: 10px;
    width: 250px;
    box-shadow: 0 4px 6px rgba(0,0,0,0.1);
  ">
    <h3 style="text-align:center; color:#333;">Login</h3>
    <input type="text" placeholder="Username" style="width:100%; padding:8px; margin:8px 0; border:1px solid #ccc; border-radius:4px;">
    <input type="password" placeholder="Password" style="width:100%; padding:8px; margin:8px 0; border:1px solid #ccc; border-radius:4px;">
    <button style="width:100%; padding:8px; background:#0072ff; color:white; border:none; border-radius:4px;">Login</button>
  </div>
</div>
""")

```





<div style="
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  background: linear-gradient(to right, #00c6ff, #0072ff);
  font-family: Arial, sans-serif;
">
  <div style="
    background: white;
    padding: 20px;
    border-radius: 10px;
    width: 250px;
    box-shadow: 0 4px 6px rgba(0,0,0,0.1);
  ">
    <h3 style="text-align:center; color:#333;">Login</h3>
    <input type="text" placeholder="Username" style="width:100%; padding:8px; margin:8px 0; border:1px solid #ccc; border-radius:4px;">
    <input type="password" placeholder="Password" style="width:100%; padding:8px; margin:8px 0; border:1px solid #ccc; border-radius:4px;">
    <button style="width:100%; padding:8px; background:#0072ff; color:white; border:none; border-radius:4px;">Login</button>
  </div>
</div>





```python
HTML("""
<div style="
  max-width: 250px;
  margin: 40px auto;
  padding: 20px;
  background: white;
  border-radius: 12px;
  box-shadow: 0 6px 10px rgba(0,0,0,0.1);
  text-align: center;
  font-family: sans-serif;
">
  <img src="https://via.placeholder.com/100" style="border-radius: 50%;" />
  <h3>John Doe</h3>
  <p style="color: gray;">Web Developer</p>
</div>
""")

```





<div style="
  max-width: 250px;
  margin: 40px auto;
  padding: 20px;
  background: white;
  border-radius: 12px;
  box-shadow: 0 6px 10px rgba(0,0,0,0.1);
  text-align: center;
  font-family: sans-serif;
">
  <img src="https://via.placeholder.com/100" style="border-radius: 50%;" />
  <h3>John Doe</h3>
  <p style="color: gray;">Web Developer</p>
</div>





```python
HTML("""
<div style="
  height: 100vh;
  background: linear-gradient(135deg, #667eea, #764ba2);
  color: white;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: sans-serif;
  font-size: 24px;
">
  Welcome to My Gradient Page
</div>
""")

```





<div style="
  height: 100vh;
  background: linear-gradient(135deg, #667eea, #764ba2);
  color: white;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: sans-serif;
  font-size: 24px;
">
  Welcome to My Gradient Page
</div>





```python
HTML("""
<div style="text-align:center; margin-top: 100px;">
  <div style="
    border: 6px solid #f3f3f3;
    border-top: 6px solid #3498db;
    border-radius: 50%;
    width: 60px;
    height: 60px;
    animation: spin 1s linear infinite;
    margin: auto;
  "></div>
  <style>
    @keyframes spin {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }
  </style>
  <p style="font-family:sans-serif;">Loading...</p>
</div>
""")

```





<div style="text-align:center; margin-top: 100px;">
  <div style="
    border: 6px solid #f3f3f3;
    border-top: 6px solid #3498db;
    border-radius: 50%;
    width: 60px;
    height: 60px;
    animation: spin 1s linear infinite;
    margin: auto;
  "></div>
  <style>
    @keyframes spin {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }
  </style>
  <p style="font-family:sans-serif;">Loading...</p>
</div>





```python
from IPython.display import HTML

HTML("""
<div style="background: #333; overflow: hidden; font-family: sans-serif;">
  <a href="#" style="float: left; color: white; text-align: center; padding: 14px 16px; text-decoration: none;">Home</a>
  <a href="#" style="float: left; color: white; text-align: center; padding: 14px 16px; text-decoration: none;">About</a>
  <a href="#" style="float: left; color: white; text-align: center; padding: 14px 16px; text-decoration: none;">Contact</a>
</div>
""")

```





<div style="background: #333; overflow: hidden; font-family: sans-serif;">
  <a href="#" style="float: left; color: white; text-align: center; padding: 14px 16px; text-decoration: none;">Home</a>
  <a href="#" style="float: left; color: white; text-align: center; padding: 14px 16px; text-decoration: none;">About</a>
  <a href="#" style="float: left; color: white; text-align: center; padding: 14px 16px; text-decoration: none;">Contact</a>
</div>





```python
HTML("""
<div style="display: flex; justify-content: center; gap: 10px; margin-top: 30px;">
  <img src="https://via.placeholder.com/100" style="border-radius: 8px;">
  <img src="https://via.placeholder.com/100" style="border-radius: 8px;">
  <img src="https://via.placeholder.com/100" style="border-radius: 8px;">
</div>
""")

```





<div style="display: flex; justify-content: center; gap: 10px; margin-top: 30px;">
  <img src="https://via.placeholder.com/100" style="border-radius: 8px;">
  <img src="https://via.placeholder.com/100" style="border-radius: 8px;">
  <img src="https://via.placeholder.com/100" style="border-radius: 8px;">
</div>





```python
HTML("""
<div style="max-width: 300px; margin: 30px auto; font-family: sans-serif;">
  <h3>Contact Us</h3>
  <input type="text" placeholder="Your Name" style="width:100%; padding:8px; margin:6px 0;"><br>
  <input type="email" placeholder="Your Email" style="width:100%; padding:8px; margin:6px 0;"><br>
  <textarea placeholder="Your Message" style="width:100%; padding:8px; margin:6px 0;"></textarea><br>
  <button style="padding:10px; background:#007bff; color:white; border:none; border-radius:5px;">Send</button>
</div>
""")

```





<div style="max-width: 300px; margin: 30px auto; font-family: sans-serif;">
  <h3>Contact Us</h3>
  <input type="text" placeholder="Your Name" style="width:100%; padding:8px; margin:6px 0;"><br>
  <input type="email" placeholder="Your Email" style="width:100%; padding:8px; margin:6px 0;"><br>
  <textarea placeholder="Your Message" style="width:100%; padding:8px; margin:6px 0;"></textarea><br>
  <button style="padding:10px; background:#007bff; color:white; border:none; border-radius:5px;">Send</button>
</div>





```python
HTML("""
<div style="background: #222; color: #ccc; text-align: center; padding: 20px; font-family: sans-serif; margin-top: 40px;">
  &copy; 2025 My Website | <a href="#" style="color:#00bfff; text-decoration: none;">Privacy Policy</a>
</div>
""")

```





<div style="background: #222; color: #ccc; text-align: center; padding: 20px; font-family: sans-serif; margin-top: 40px;">
  &copy; 2025 My Website | <a href="#" style="color:#00bfff; text-decoration: none;">Privacy Policy</a>
</div>





```python
from IPython.display import HTML

HTML("""
<div style="font-family: Arial, sans-serif;">
  <button onclick="this.nextElementSibling.style.display = 
    this.nextElementSibling.style.display === 'block' ? 'none' : 'block';"
    style="background-color: #007bff; color: white; padding: 10px; border: none; width: 100%; text-align: left;">
    What is BGMI?
  </button>
  <div style="display: none; padding: 10px; background-color: #f1f1f1;">
    BGMI stands for Battlegrounds Mobile India. It’s a popular mobile game by Krafton.
  </div>
</div>
""")

```





<div style="font-family: Arial, sans-serif;">
  <button onclick="this.nextElementSibling.style.display = 
    this.nextElementSibling.style.display === 'block' ? 'none' : 'block';"
    style="background-color: #007bff; color: white; padding: 10px; border: none; width: 100%; text-align: left;">
    What is BGMI?
  </button>
  <div style="display: none; padding: 10px; background-color: #f1f1f1;">
    BGMI stands for Battlegrounds Mobile India. It’s a popular mobile game by Krafton.
  </div>
</div>





```python

```





<div style="
  width: 250px; 
  height: 150px; 
  border-radius: 10px; 
  padding: 20px; 
  color: white; 
  font-family: sans-serif;
  background: linear-gradient(45deg, #ff6ec4, #7873f5);
  animation: gradient 4s ease infinite;
">
  <h4>Gradient Box</h4>
  <p>This box has a moving gradient!</p>
</div>

<style>
@keyframes gradient {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}
div[style*="gradient"] {
  background-size: 200% 200%;
}
</style>





```python
from IPython.core.display import display, HTML

html_card = """
<div style="width: 200px; padding: 15px; background-color: #fff; border: 1px solid #ddd; box-shadow: 2px 2px 8px rgba(0,0,0,0.1); border-radius: 10px;">
  <h4>Title</h4>
  <p>This is a simple card box.</p>
</div>
"""

display(HTML(html_card))


```

    C:\Users\sahil\AppData\Local\Temp\ipykernel_2864\1854938944.py:1: DeprecationWarning: Importing display from IPython.core.display is deprecated since IPython 7.14, please import from IPython.display
      from IPython.core.display import display, HTML
    



<div style="width: 200px; padding: 15px; background-color: #fff; border: 1px solid #ddd; box-shadow: 2px 2px 8px rgba(0,0,0,0.1); border-radius: 10px;">
  <h4>Title</h4>
  <p>This is a simple card box.</p>
</div>




```python
tags_html = """
<span style="background-color: #ffeb3b; padding: 5px 10px; border-radius: 20px; font-size: 14px;">HTML</span>
<span style="background-color: #8bc34a; padding: 5px 10px; border-radius: 20px; font-size: 14px;">CSS</span>
<span style="background-color: #03a9f4; padding: 5px 10px; border-radius: 20px; font-size: 14px;">JS</span>
"""

display(HTML(tags_html))

```



<span style="background-color: #ffeb3b; padding: 5px 10px; border-radius: 20px; font-size: 14px;">HTML</span>
<span style="background-color: #8bc34a; padding: 5px 10px; border-radius: 20px; font-size: 14px;">CSS</span>
<span style="background-color: #03a9f4; padding: 5px 10px; border-radius: 20px; font-size: 14px;">JS</span>




```python

```


---
**Score: 45**