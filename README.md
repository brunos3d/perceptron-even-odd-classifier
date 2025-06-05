# 🧠 Perceptron Visualizer: Even or Odd Classifier

This project is an interactive JavaScript visualization of a perceptron neural network that learns to classify numbers as **even or odd**. It provides a live, browser-based interface with visualization powered by D3.js.

---

## 🚀 Features

- 🔍 Input a number and test if it's classified as even or odd
- 🧠 Visual graph of the neural network structure (input → neuron → output)
- ⚙️ Train automatically until reaching a target accuracy
- ⏹️ Stop training at any time
- 📊 Live display of weights, bias, epoch count, and accuracy

---

## 📚 How It Works

This project uses a **single-layer perceptron** — the simplest form of a neural network — to classify numbers.

### 🧮 Perceptron Equation

The perceptron calculates the output `y` from input `x` using:

```
y = f(w * x + b)
```

Where:
- `x` is the input (in this case, `x = n % 2`)
- `w` is the weight
- `b` is the bias
- `f(z)` is the activation function:
  ```
  f(z) = {
    1, if z >= 0.5
    0, otherwise
  }
  ```

The output `y` will be:
- `1` for odd numbers
- `0` for even numbers

### 🔁 Training Rule

Each epoch updates weights using the perceptron learning rule:

```
error = expected - predicted
w = w + learningRate * error * x
b = b + learningRate * error
```

This update process is repeated until the accuracy reaches a user-defined threshold.

---

## 🎨 Visualization

D3.js is used to render a simple visual of the perceptron network:
- **Input Node**
- **Single Neuron**
- **Output Node**

These are connected with lines and display live updates of current weights and bias.

---

## 🧪 Usage

1. Open `index.html` in your browser.
2. Enter a minimum accuracy (default: 90%).
3. Click **Train Perceptron**.
4. The network will train until the desired accuracy is reached.
5. Use **Test Number** to verify the classification of any integer.
6. Click **Stop Training** to manually halt training.

---

## 🛠 Tech Stack

- **HTML5**
- **JavaScript (Vanilla)**
- **D3.js v7**

No build tools or dependencies required — just open the HTML file in your browser.

---

## 🧠 Educational Purpose

This project is meant as a learning tool to demonstrate:
- How perceptrons work
- Binary classification
- Live training feedback
- Basic D3.js visualizations

---

## 📄 License

MIT — Free to use, modify, and share.
