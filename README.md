# Pop Quiz Detais

## Setup
```
$ Open Terminal
$ mkdir ~/work/github
$ cd ~/work/github
$ git clone https://github.com/gsypolt/pop-quiz-two.git
$ bundle
$ cucumber --tags @quiz1

```


## Quiz 1:
For this pop quiz you will be using a scenario outline to navigate all the top level fronts and validate that correct front appears. 

Specs: 
* Open Browser > mhigh.usatoday.com > Click Menu Button
* Inspect element for each section menu item (Home, News, Sports, etc.) and capture the HTML attribute "href" for each section

Gherkin Description:
* Go directly to each section front with out using the clicking workflow by passing the captured "href" base_url(path) (i.e. mhigh.usatoday.com/news/)
* Add an assertion to validate correct front appears (hint: header/banner class)


## Quiz 2:
For this pop quiz you will be using a scenario outline to navigate Videos & Photos then validate user can filter and only see filter media appear on screen.

Specs:
* Open Browser > mhigh.usatoday.com/media/ > (Top Left) Filter
* Inspect element for each media type filter and media icon (video or photo)

Gherkin Description:
* Go directly to Videos & Photos section.
* Change filter to videos only, photos only, and filter all
* Add an assertion to validate media item appearing on screen matches the filter option selected (video only, photo only, or both)