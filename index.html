<?php
try {
        $url = 'https://dynamicdns.park-your-domain.com/update?host='.$_GET['host'].'&domain='.$_GET['domain'].'&password='.$_GET['password'].'&ip='.$_GET['ip'];
        $req = curl_init();
        curl_setopt($req, CURLOPT_URL, $url);
        curl_setopt($req, CURLOPT_RETURNTRANSFER, true);
        curl_setopt($ch, CURLOPT_HTTPHEADER, array('Content-type: text/xml'));
        $res = curl_exec($req);
        curl_close($req);
        $xml = new SimpleXMLElement(trim(str_replace("encoding=\"utf-16\"","",$res)));
        if ($xml->ErrCount > 0) {
                $error = $xml->errors[0]->Err1;
                if (strcmp($error, "Domain name not found") === 0) {
                        echo "nohost";
                } elseif (strcmp($error, "Passwords do not match") === 0) {
                        echo "badauth";
                } elseif (strcmp($error, "No Records updated. A record not Found;") === 0) {
                        echo "nohost";
                } else {
                   echo "911 [".$error."]";
                }
        } else {
                echo "good";
        }
} catch (Exception $e) {
    echo "911 [".$e->getMessage()."]";
}
