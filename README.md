# elasticsearch-isalive A plugin which checks cluster health status

[elasticsearch-isalive](https://github.com/liip/elasticsearch-isalive)

An elastic search site plugin which checks the cluster health status and repondes "Is up and Running!" for status "green" or "yellow". Otherwise it will respond with: "is gone!".

This plugin can be used for loadbalancers to determin if a node is up and running.

## Installing and Running

### Running as a plugin of ElasticSearch

	sudo elasticsearch/bin/plugin -install liip/elasticsearch-isalive
	open http://localhost:9200/_plugin/isalive/

This will automatically download the latest version of elasticsearch-isalive from github and run it as a plugin within the elasticsearch cluster. In this mode:

- elasticsearch provides a simple webserver to run head
- elasticsearch-isalive automatically connects to the node that is running it
- is available at http://localhost:9200/_plugin/isalive/ (or whatever the address of your cluster is)


### URL Parameters

currently none

