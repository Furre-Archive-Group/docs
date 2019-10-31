# "current" news file
All lines are key/value entries seperated by a space.\
First line should have a `NewsVersion` key, followed by a float of the format version.
Lines should be seperated by `\r\n`. File should end with `\r\n`.

## Version 1
### Confirm
Should contain a unique hash(32 hex characters long). Used to verify that the user has seen the latest news.

### ForceClose
Either `yes` or `no`. If yes, forces the news window to close.

### ForceForeground
Either `yes` or `no`. If yes, forces the news window to the foreground.

### ForceOpen
Either `yes` or `no`. If yes, forces the news window to open, even if the user has seen the latest news.

### ForceURL
Either `none` or a url. If not none, forces the url to open in a browser window.

### NewsID
Should contain a unique hash(32 hex characters long). Used to see if the news has updated.

### NewsDate
Date of which the news was last updated. Format is `YYYY-MM-DD HH:MM:SS` in UTC 24-hour time.

### NewsEntry
A tab(`\t`) seperated entry containing the following values in this order:

#### Human Readable Date
Space seperated value of sort month, day, year. EG: Oct 18, 2019

#### Unknown
Integer, set to `0`.

#### Category
One of:
* General
* Updates
* Events
* Digo Market

#### Title
News entry title

#### Body
News entry body. New lines are represented by `#LF#`

#### URL
Either empty or a URL. Used for the "Read more" button.

#### Image
Either empty or a URL. Used to display a image on the left side. Max 100x100 pixels.