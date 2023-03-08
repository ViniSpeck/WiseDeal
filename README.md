# WiseDeal
![image](https://user-images.githubusercontent.com/69943624/223627754-4db1a412-4956-470a-8c32-24157098bead.png)


This is a Python application that receives data on products and prices from various stores through an API, normalizes and loads it into a datalake as raw data. It extracts, transforms, and loads the raw data daily and stores the data on a data warehouse. Upon user request, the application queries the price of an item at a particular moment and presents a graph of the price history of that item. It also evaluates through a machine learning model whether it is worth buying the item currently at the store with the lowest price or whether the trend is for the price of the item to decrease.


## Requirements

- Python 3.6 or higher
- Docker
- Docker Compose

## Installation

1. Clone the repository:

  `git clone https://github.com/<username>/<repository-name>.git`

2. Navigate to the project root directory:

  `cd <repository-name>`

3. Build the Docker image:

  `docker-compose build`

4. Start the containers:

  `docker-compose up -d`

This will start the containers in the background.

## Usage

1. Access the web interface by navigating to `http://localhost:8000` in your web browser.

2. Select a category of items from the dropdown menu.

3. Select an item from the list of popular items in that category.

4. Click the "Get Price History" button to see a graph of the price history for that item.

5. The machine learning model will automatically evaluate whether it is worth buying the item currently at the store with the lowest price or whether the trend is for the price of the item to decrease.

## Contributing

We welcome contributions to this project. To contribute:

1. Fork the repository.

2. Create a new branch:

  `git checkout -b <branch-name>`

3. Make your changes and commit them:

  `git commit -am 'Add some feature'`

4. Push to the branch:

  `git push origin <branch-name>`

5. Create a new pull request.

## Testing

To run tests, navigate to the project root directory and run:

  `docker-compose run web python manage.py test`

This will run the tests for the application.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
