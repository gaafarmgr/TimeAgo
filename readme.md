#TimeAgo
##Overview
TimeAgo generates 'friendly' elapsed time sentences, based on PHPs [DateTime](http://php.net/datetime) classes.

##usage
Include the file into your project and instantiate, passing in a DateTime object representing a time in the past:-

    include 'TimeAgo.php';
    $pastTime = new \DateTime('Some time in the past);
    $timeAgo = new TimeAgo($pastTime);
    echo $timeAgo . " ago<br/>\n";

This will give an output something like:-

    16 hours 14 minutes 38 seconds ago

##Methods
###`__toString()`
Magic method. Returns the formated string.

###`setInterval(\DateInterval $interval)`
Sets TimeAgo to a specific DateInterval. Handy for testing.
