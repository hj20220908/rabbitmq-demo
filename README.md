<pre><code>
sudo docker run -d --name rabbitmq -p 5672:5672 -p 15672:15672 \
                   --restart=unless-stopped \
                   -e RABBITMQ_DEFAULT_USER=root \
                   -e RABBITMQ_DEFAULT_PASS=root \
                   rabbitmq:management

http://127.0.0.1:15672
</code></pre>