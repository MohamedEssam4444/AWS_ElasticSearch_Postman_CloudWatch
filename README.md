# AWS_ElasticSearch_Postman_CloudWatch
uploading document to AWS ElasticSearch service using linux and Postman and seeing visuals on CloudWatch

## Files
1. **elasticsearch commands.sh**: Containing commands used on linux for elastics search get and post records

2. **bulk_veggies.json**: Containing couple of records used for _bulk POST 

### Screenshots
1. **Making Amazon Elastic Search Cluster**
![Screenshot from 2020-12-19 11-37-22](https://user-images.githubusercontent.com/68178003/102689578-d921b000-4207-11eb-8416-3dd4c64085ba.png)

![Screenshot from 2020-12-19 11-38-39](https://user-images.githubusercontent.com/68178003/102689579-dcb53700-4207-11eb-8c81-2e66a7707dc6.png)

![Screenshot from 2020-12-19 12-36-27](https://user-images.githubusercontent.com/68178003/102689581-e048be00-4207-11eb-97eb-facc4d17e2bf.png)

![Screenshot from 2020-12-19 12-36-51](https://user-images.githubusercontent.com/68178003/102689995-281d1480-420b-11eb-95cc-3edff9e10891.png)

![Screenshot from 2020-12-19 13-06-10](https://user-images.githubusercontent.com/68178003/102689997-2b180500-420b-11eb-8ffb-34b4b2492523.png)

2. **Using Postman to post and get document**

![Screenshot from 2020-12-19 13-12-19](https://user-images.githubusercontent.com/68178003/102690000-2e12f580-420b-11eb-8847-77f400618ab0.png)

![Screenshot from 2020-12-19 13-12-44](https://user-images.githubusercontent.com/68178003/102690002-3408d680-420b-11eb-819a-66083f7f4faf.png)

![Screenshot from 2020-12-19 13-13-11](https://user-images.githubusercontent.com/68178003/102690004-379c5d80-420b-11eb-9e5c-72c50dec0bb0.png)

3. **Using elasticsearch Commands on linux to get info about cluster**

![Screenshot from 2020-12-19 13-46-54](https://user-images.githubusercontent.com/68178003/102690008-3bc87b00-420b-11eb-8cc1-a560ec6cc9b1.png)

* **using this command to make a bulk post with many records to the document using bulk_veggies.json file**
`curl -XPOST 'https://search-mohamedessam-tazcrwadnhfehyo5jsqmc5bobm.us-west-2.es.amazonaws.com/_bulk' --data-binary @bulk_veggies.json -H 'Content-Type: application/json'`

* **Search for lettuce vegetable record with this command**
` curl -XGET 'https://search-mohamedessam-tazcrwadnhfehyo5jsqmc5bobm.us-west-2.es.amazonaws.com/veggies/_search?q=name:l*?pretty'`

![Screenshot from 2020-12-19 14-01-25](https://user-images.githubusercontent.com/68178003/102690013-4125c580-420b-11eb-9b84-487a7ec51d44.png)

4. **searching for some records using id**
![Screenshot from 2020-12-19 14-05-47](https://user-images.githubusercontent.com/68178003/102690015-4551e300-420b-11eb-8eb8-0d3e9df243db.png)

![Screenshot from 2020-12-19 14-28-14](https://user-images.githubusercontent.com/68178003/102690030-5569c280-420b-11eb-9b01-519bc23388fb.png)

5. **Checking AWS console**

![Screenshot from 2020-12-19 14-11-52](https://user-images.githubusercontent.com/68178003/102690018-484cd380-420b-11eb-81b1-2ef3afce8c2f.png)

6. **CloudWatch Visuals**

![Screenshot from 2020-12-19 14-13-47](https://user-images.githubusercontent.com/68178003/102690039-64507500-420b-11eb-940f-a4f330f4a15d.png)

![Screenshot from 2020-12-19 14-14-21](https://user-images.githubusercontent.com/68178003/102690044-703c3700-420b-11eb-8a3d-54d2f48618dd.png)

![Screenshot from 2020-12-19 14-14-34](https://user-images.githubusercontent.com/68178003/102690047-7500eb00-420b-11eb-96cd-f86119e2cfb5.png)

![Screenshot from 2020-12-19 14-16-11](https://user-images.githubusercontent.com/68178003/102690054-792d0880-420b-11eb-831c-5e7252448f60.png)

![Screenshot from 2020-12-19 14-16-25](https://user-images.githubusercontent.com/68178003/102690056-7cc08f80-420b-11eb-9499-ee1d5e7bd87a.png)

![Screenshot from 2020-12-19 14-16-57](https://user-images.githubusercontent.com/68178003/102690058-80541680-420b-11eb-8216-5f18ba7386ef.png)
