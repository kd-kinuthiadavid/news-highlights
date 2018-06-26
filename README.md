# NEWS HIGHLIGHTS

An application that previews news articles from  various sources.

## Getting Started

These instructions will get you  a copy of the project up  and running on your local machine  for development and testing  purposes:

```
open your terminal
```

```
git clone https://github.com/kd-kinuthiadavid/news-highlights.git

```
```
cd news-highlights

```
To activate  virtual environment:

```
$ sudo apt-get install python3.6-venv

```

```
$ python3.6 -m venv virtual

```
```
$ source virtual/bin/activate

```

See deployment for notes on how to deploy the project on a live system.

### Prerequisites

No installation required, just follow the link below to get to this application:
[News Highlights]( https://github.com/kd-kinuthiadavid/news-highlights.git)


### Installation

A step by step series of examples that tell you how to get a development environment running:

* Refer to the Getting Started section

## Running the tests

Explains how to run the automated tests for this system:

* navigate to where the application is located in your development environment, refer to the Installation section if you don't have a development environment and would like one.

* run the following command.

```
python3.6 manage.py test

```

### End to end tests

Tests the behaviour of the News Sources

```
class News_sources_Test(unittest.Testcase):
    """
    Test Class to test the behaviour of the News_sources class
    """
    def setup(self):
        '''
        Set up method that will run before every Test
        '''
        self.news_sources = News_sources('the-new-york-times', 'The New York Times', 'Charles V. Bagli and Jesse Drucker', 'Vornado Realty Trust\u2019s chairman said it had agreed to sell its part of the financially troubled building to the Kushners.', 'www.nytimes.com/2018/04/06/nyregion/kushners-vornado-666-fifth-avenue.html')

    def test_instance(self):
        self.assertTrue(isinstance(self.new_source, News_source))

```

## Deployment

Additional notes about how to deploy this on a live system:

* install gunicorn
```
(virtual)$ python3.6 -m  pip install gunicorn

```
* create a free heroku [account](https://signup.heroku.com/)

* deploy:

```
$ git add .
$ git commit -m "deployment to heroku"
$ git push heroku master
```

## Built With

* Python3.6
* Flask



## Authors

* **KINUTHIA DAVID**

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to my TM's at Moringa School
