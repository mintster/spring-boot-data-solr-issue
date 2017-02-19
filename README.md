##Spring Boot Sample Data Solr

Demonstrates duplicate Core Names added in Solr Url in Spring Boot 1.5.1

See issue:  [#8327](https://github.com/spring-projects/spring-boot/issues/8327)

####Result of running `SampleSolrApplicationTests`:

```html
<head>
<meta http-equiv="Content-Type" content="text/html; charset=UTF-8"/>
<title>Error 404 Not Found</title>
</head>
<body><h2>HTTP ERROR 404</h2>
<p>Problem accessing /solr/collection1/collection1/update. Reason:
<pre>    Not Found</pre></p><hr><i><small>Powered by Jetty://</small></i><hr/>

</body>
</html>
; nested exception is org.apache.solr.client.solrj.impl.HttpSolrClient$RemoteSolrException: Error from server at http://127.0.0.1:8983/solr/collection1: Expected mime type application/octet-stream but got text/html. <html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=UTF-8"/>
<title>Error 404 Not Found</title>
</head>
<body><h2>HTTP ERROR 404</h2>
<p>Problem accessing /solr/collection1/collection1/update. Reason:
<pre>    Not Found</pre></p><hr><i><small>Powered by Jetty://</small></i><hr/>

</body>
</html>
```