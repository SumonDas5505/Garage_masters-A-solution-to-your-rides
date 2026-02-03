# GarageMaster – A Solution to Your Rides
Overview

GarageMaster is an e‑commerce platform built to make purchasing car and bike modification parts easier. The project includes a front‑end website with features such as product catalog, search and category filtering, custom package builder, shopping cart with currency conversion, voucher system, user authentication and more. A separate research notebook explores a hybrid quantum–classical neural network using Qiskit and PyTorch. Throughout the project the team applied several software design patterns to improve code maintainability and extensibility.

Features

Responsive front‑end: A user‑friendly HTML/CSS/JavaScript interface presents lists of car and bike accessories. The site includes search and sorting components and dynamically updates the shopping cart.

Category search & strategy pattern: The file searchStrategy.js defines a SearchStrategy class with methods to show all products or filter them by category; the appropriate strategy is selected when the user chooses a category.

Packages (composite pattern): On the home page users can build sets of bike or car packages by incrementing or decrementing quantities; each package lists several accessories and displays the total price.

Cart with currency conversion (adapter pattern): The cart page uses an ExternalCurrencyService with a hard‑coded exchange rate and a CurrencyAdapter to convert prices from BDT to USD; totals are shown in both currencies.

Voucher system (factory pattern): A VoucherFactory creates a voucher worth ৳500 for orders over ৳5000. The cart applies this voucher and updates the order summary accordingly.

User authentication (singleton pattern): The UserManager class follows the singleton pattern to ensure there is only one instance managing users. It stores registered users and the current signed‑in user in localStorage and exposes functions for registration, sign‑in and logout.

Search and sorting: Users can filter products by keywords using the search bar and there are placeholders for sorting and number‑of‑items controls.

Quantum ML notebook: The repository includes HQCNN_ANIK.ipynb, a research notebook that installs Qiskit, Qiskit‑Aer and other machine‑learning libraries. The notebook demonstrates a hybrid quantum–classical convolutional neural network for image classification.

Technology stack

Front‑end: HTML, CSS, JavaScript, localStorage.

Design patterns: Strategy, Singleton, Composite, Adapter, Factory and (originally) Decorator for applying discounts.

Research: Python, Qiskit, PyTorch, scikit‑learn for the hybrid quantum neural network.

Setup & running

Clone the repository: Clone or download the project to your local machine.

Launch the website: Open index.html in a web browser to browse products and build packages. Use signin.html to register or log in; user information is stored in the browser’s localStorage.

Add items to the cart: Select products or packages and add them to the cart. The cart shows totals in BDT and USD using the currency adapter and automatically applies a voucher when eligible.

Explore the quantum notebook: Open HQCNN_ANIK.ipynb in Jupyter Notebook or Google Colab. The first cell installs the required dependencies; follow the notebook to experiment with the hybrid quantum–classical neural network.

Contributing

This project was developed for an academic course and is not actively maintained. Nevertheless, feedback and contributions are welcome. Feel free to fork the repository and submit pull requests for improvements or bug fixes.

License

Specify a suitable open‑source license (e.g., MIT License) if you intend to share the project publicly. Without a license, the code is open for educational use only.
