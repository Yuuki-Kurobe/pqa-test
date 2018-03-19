<?php
$data = "https://spreadsheets.google.com/feeds/list/GoogleスプレッドシートのIDを入力/od6/public/values?alt=json";
$json = file_get_contents($data);
$json_decode = json_decode($json);

$names = $json_decode->feed->entry;

foreach ($names as $name) {
    echo $name->{'gsx$speech'}->{'$t'};
    echo $name->{'gsx$displayText'}->{'$t'};
        echo ",";
}
