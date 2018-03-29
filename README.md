# AWS_IOT_Create_and_Access_Thing_UsingMQTT

below are some steps to create your IOT thing using AWS.


`Create a policy provide name,Action,Resource ARN,Effect then Create.`
![Throughput Graph](https://github.com/PiyushMittl/AWS_IOT_Create_and_Access_Thing_UsingMQTT/blob/master/im1_create_policy.png)


`AWS Iot->Create`
![Throughput Graph](https://github.com/PiyushMittl/AWS_IOT_Create_and_Access_Thing_UsingMQTT/blob/master/im2_create.png)


`Give a Thing name.`
![Throughput Graph](https://github.com/PiyushMittl/AWS_IOT_Create_and_Access_Thing_UsingMQTT/blob/master/im2_give_thing_name.png)


`After giving thing name click on Create thing.`
![Throughput Graph](https://github.com/PiyushMittl/AWS_IOT_Create_and_Access_Thing_UsingMQTT/blob/master/im4_create_thing.png)


`After creating a thing you will get redirect to above page.`
![Throughput Graph](https://github.com/PiyushMittl/AWS_IOT_Create_and_Access_Thing_UsingMQTT/blob/master/im5_page_redirect.png)


`Click on security->create certificate`
![Throughput Graph](https://github.com/PiyushMittl/AWS_IOT_Create_and_Access_Thing_UsingMQTT/blob/master/im6_create_certificate.png)


`Click on Activate.`
![Throughput Graph](https://github.com/PiyushMittl/AWS_IOT_Create_and_Access_Thing_UsingMQTT/blob/master/im7_activate.png)


`Download all the keys.`
![Throughput Graph](https://github.com/PiyushMittl/AWS_IOT_Create_and_Access_Thing_UsingMQTT/blob/master/im8_download_keys.png)


`Click on Attach a Policy`
![Throughput Graph](https://github.com/PiyushMittl/AWS_IOT_Create_and_Access_Thing_UsingMQTT/blob/master/im9_attach_policy.png)

`Attach previously created policy`
![Throughput Graph](https://github.com/PiyushMittl/AWS_IOT_Create_and_Access_Thing_UsingMQTT/blob/master/im10_attach_previously_created_ploicy.png)


`Now goto thing`
![Throughput Graph](https://github.com/PiyushMittl/AWS_IOT_Create_and_Access_Thing_UsingMQTT/blob/master/im11_goto_thing.png)


`Shadow->delete`
![Throughput Graph](https://github.com/PiyushMittl/AWS_IOT_Create_and_Access_Thing_UsingMQTT/blob/master/im12_delete_shadow.png)


`Create shadow document`
![Throughput Graph](https://github.com/PiyushMittl/AWS_IOT_Create_and_Access_Thing_UsingMQTT/blob/master/im12_create_shadow_document.png)

```
Connecting a thing with MQTT
Go to
http://docs.aws.amazon.com/iot/latest/developerguide/managing-device-certs.html
```
![Throughput Graph](https://github.com/PiyushMittl/AWS_IOT_Create_and_Access_Thing_UsingMQTT/blob/master/im13.png)


`Click on underlined link`
![Throughput Graph](https://github.com/PiyushMittl/AWS_IOT_Create_and_Access_Thing_UsingMQTT/blob/master/im14.png)

```
You will be redirected to the above screen.
Copy the stuff and paste to a file 
Save that file with extension .pem
I have saved that file as 
VeriSign-Class 3-Public-Primary-Certification-Authority-G5.pem
```
![Throughput Graph](https://github.com/PiyushMittl/AWS_IOT_Create_and_Access_Thing_UsingMQTT/blob/master/im15.png)



`Click on highlighted symbol`
![Throughput Graph](https://github.com/PiyushMittl/AWS_IOT_Create_and_Access_Thing_UsingMQTT/blob/master/im16.png)

```
Give Broker Addredd and port then Generate client id
You will get Broker address from your IOT thing 
```
![Throughput Graph](https://github.com/PiyushMittl/AWS_IOT_Create_and_Access_Thing_UsingMQTT/blob/master/im17.png)


![Throughput Graph](https://github.com/PiyushMittl/AWS_IOT_Create_and_Access_Thing_UsingMQTT/blob/master/im18.png)

![Throughput Graph](https://github.com/PiyushMittl/AWS_IOT_Create_and_Access_Thing_UsingMQTT/blob/master/im19.png)

```
Click on SSL/TLS
Provide 
CA file previously created 
Client Certificate file previously downloaded
Client private key previously downloaded
Check PEM formatted
Now click on okay.
```
![Throughput Graph](https://github.com/PiyushMittl/AWS_IOT_Create_and_Access_Thing_UsingMQTT/blob/master/im20.png)

```
Click on connect 
After connecting the light given at right most corner will become green
```
![Throughput Graph](https://github.com/PiyushMittl/AWS_IOT_Create_and_Access_Thing_UsingMQTT/blob/master/im21.png)