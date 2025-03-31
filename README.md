<!DOCTYPE html>
<html lang="en">

<head>
  <title>My First HTML Page</title>
</head>
<body>
  <header>
    <h1>Welcome to My Web Page</h1>
  </header>
<nav>
    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <main>
    <section id="home">
      <h2>Home</h2>
      <p>Welcome to my awesome webpage!</p>
    </section>

    <section id="about">
      <h2>About</h2>   
      <p>This page is created using HTML5 semantic elements for better structure and accessibility.</p>
    </section>
  </main>

  <footer>
    <p>Contact us at: 
      <a href="https://www.linkedin.com/in/voice-of-reason-njoki-93412021b/" blank_="">Linkedin</a>
      <a href="email to="doreenjoki98@gmail.com" blank_=""> Email </a>
    </p>
  </footer>
</body>

</html>






def basic_calculator():
    print("==== BASIC PYTHON CALCULATOR ====")
    
    try:
        num1 = float(input("Enter first number: "))
        operator = input("Enter operator (+, -, *, /): ")
        num2 = float(input("Enter second number: "))
        
        if operator == "+":
            result = num1 + num2
        elif operator == "-":
            result = num1 - num2
        elif operator == "*":
            result = num1 * num2
        elif operator == "/":
            if num2 == 0:
                print("Error: Can't divide by zero!")
                return
            result = num1 / num2
        else:
            print("Error: Invalid operator! Use +, -, *, or /")
            return
        
        print(f"Result: {num1} {operator} {num2} = {result}")
    
    except ValueError:
        print("Error: Please enter valid numbers!")

# Run the calculator
basic_calculator()