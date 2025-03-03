# luckdata-instagram-api-free
luckdata Instagram API , The most stable and fastest Instagram API on the web, you can use it to get Instagram user profiles, post details, search and more. We will consistently maintain and update it to make your work more convenient.
# How to Use

Step 1: Click “Get Started”

Step 2: Purchase a plan and complete the payment

Step 3: Choose your preferred run mode

Step 4: Click "Test Endpoint"

# How to get a free Luckdata instagram API key

Register for a Luckdata account and apply for the instagram API. Luckdata will grant 100 free points for one month, which can be used with a limit of one request per second. If you need higher points and more request capacity, a paid version is required. Alternatively, you can wait for the next month to receive another 100 free points for use.

# GET instagram Profile Code Snippets
## Python
<pre>import requests

headers = {
    'X-Luckdata-Api-Key': 'your_LuckData_api_key'
}

json_data={}

response = requests.get(
    '/api/instagram-api/profile_info?username_or_id_or_url=luckproxy',
    headers=headers,
    
)
print(response.json())</pre>
## Java
<pre>import java.io.IOException;
import java.net.URI;
import java.net.http.HttpClient;
import java.net.http.HttpRequest;
import java.net.http.HttpResponse;

HttpClient client = HttpClient.newHttpClient();

HttpRequest request = HttpRequest.newBuilder()
    .uri(URI.create("/api/instagram-api/profile_info?username_or_id_or_url=luckproxy"))
    .GET()
    
    .setHeader("X-Luckdata-Api-Key", "your_LuckData_api_key")
    .build();

HttpResponse<String> response = client.send(request, HttpResponse.BodyHandlers.ofString());</pre>
## go
<pre>package main

import (
  "fmt"
  "io"
  "log"
  "net/http"
  "strings"
)

func main() {
  client := &http.Client{}
  var data = nil
  req, err := http.NewRequest("GET", "/api/instagram-api/profile_info?username_or_id_or_url=luckproxy", data)
  if err != nil {
    log.Fatal(err)
  }
  
  req.Header.Set("X-Luckdata-Api-Key", "your_LuckData_api_key")
  resp, err := client.Do(req)
  if err != nil {
    log.Fatal(err)
  }
  defer resp.Body.Close()
  bodyText, err := io.ReadAll(resp.Body)
  if err != nil {
    log.Fatal(err)
  }
  fmt.Printf("%s\n", bodyText)
}</pre>
## shell
<pre>curl -X GET "/api/instagram-api/profile_info?username_or_id_or_url=luckproxy"  -H "X-Luckdata-Api-Key":"your_LuckData_api_key" </pre>

mroe For more information about luckdata Instagram API, please click:<a href="https://luckdata.io/marketplace/detail/instagram-api">luckdata Instagram API</a>
