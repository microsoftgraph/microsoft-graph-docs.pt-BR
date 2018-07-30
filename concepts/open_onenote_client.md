# <a name="open-the-onenote-client"></a><span data-ttu-id="966ed-101">abrir o cliente do OneNote</span><span class="sxs-lookup"><span data-stu-id="966ed-101">Open the OneNote client</span></span>

<span data-ttu-id="966ed-102">Você pode usar a propriedade **links** de uma página ou de um bloco de anotações para abrir um aplicativo do OneNote em determinada página ou bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="966ed-102">You can use the **links** property of a page or notebook to open a OneNote application to a particular page or notebook.</span></span> 

<span data-ttu-id="966ed-103">A propriedade **links** é um objeto JSON que contém duas URLs.</span><span class="sxs-lookup"><span data-stu-id="966ed-103">The **links** property is a JSON object that contains two URLs.</span></span> <span data-ttu-id="966ed-104">As URLs abrirão a página ou o bloco de anotações no aplicativo cliente do OneNote ou no OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="966ed-104">The URLs will open the page or notebook in the OneNote client application or in OneNote Online.</span></span>

```json
{ 
    "links": {
        "oneNoteClientUrl": {
            "href": "onenote:https://..."
        },
        "oneNoteWebUrl": {
            "href": "https://..."
        }
    }
}
```

- <span data-ttu-id="966ed-105">**oneNoteClientUrl**</span><span class="sxs-lookup"><span data-stu-id="966ed-105">**oneNoteClientUrl**</span></span> 

    - <span data-ttu-id="966ed-106">Abre o cliente do OneNote, caso já esteja instalado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="966ed-106">oneNoteClientUrl - Opens the OneNote client if it is already installed on the device.</span></span> <span data-ttu-id="966ed-107">Essa URL inclui o prefixo *onenote*.</span><span class="sxs-lookup"><span data-stu-id="966ed-107">This URL includes the *onenote* prefix.</span></span>
    - <span data-ttu-id="966ed-108">Abre a versão de idioma específico, caso esteja instalada no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="966ed-108">Opens the language-specific version if one is installed on the device.</span></span> <span data-ttu-id="966ed-109">Caso contrário, usa a configuração de idioma da plataforma.</span><span class="sxs-lookup"><span data-stu-id="966ed-109">Otherwise, uses the platform language setting.</span></span>

- <span data-ttu-id="966ed-110">**oneNoteWebUrl**</span><span class="sxs-lookup"><span data-stu-id="966ed-110">**oneNoteWebUrl**</span></span> 

    - <span data-ttu-id="966ed-111">Abre o OneNote Online, caso o navegador padrão do dispositivo dê suporte a ele.</span><span class="sxs-lookup"><span data-stu-id="966ed-111">oneNoteWebUrl - Opens OneNote Online if the default browser on the device supports it.</span></span> 
    - <span data-ttu-id="966ed-112">Usa a configuração de idioma do navegador.</span><span class="sxs-lookup"><span data-stu-id="966ed-112">Uses the browser language setting.</span></span>


<span data-ttu-id="966ed-113">A API do OneNote retorna a propriedade **links** na resposta HTTP para as seguintes operações:</span><span class="sxs-lookup"><span data-stu-id="966ed-113">The OneNote API returns the **links** property in the HTTP response for the following operations:</span></span>

- <span data-ttu-id="966ed-114">Crie uma página enviando uma solicitação [`POST pages`](../api-reference/v1.0/api/section_post_pages.md).</span><span class="sxs-lookup"><span data-stu-id="966ed-114">Create a page by sending a [`POST pages`](../api-reference/v1.0/api/section_post_pages.md) request</span></span>

- <span data-ttu-id="966ed-115">Crie um bloco de anotações enviando uma solicitação [`POST notebooks`](../api-reference/v1.0/api/onenote_post_notebooks.md).</span><span class="sxs-lookup"><span data-stu-id="966ed-115">Create a notebook by sending a [`POST notebooks`](../api-reference/v1.0/api/onenote_post_notebooks.md) request</span></span>

- <span data-ttu-id="966ed-116">Obtenha os metadados de página enviando uma solicitação [`GET pages`](../api-reference/v1.0/api/page_get.md) ou [`GET pages/{id}`](../api-reference/v1.0/api/page_get.md).</span><span class="sxs-lookup"><span data-stu-id="966ed-116">Get page metadata by sending a [`GET pages`](../api-reference/v1.0/api/page_get.md) or [`GET pages/{id}`](../api-reference/v1.0/api/page_get.md) request</span></span>

- <span data-ttu-id="966ed-117">Obtenha metadados de bloco de anotações enviando uma solicitação [`GET notebooks`](../api-reference/v1.0/api/notebook_get.md) ou [`GET notebooks/{id}`](../api-reference/v1.0/api/notebook_get.md).</span><span class="sxs-lookup"><span data-stu-id="966ed-117">Get notebook metadata by sending a [`GET notebooks`](../api-reference/v1.0/api/notebook_get.md) or [`GET notebooks/{id}`](../api-reference/v1.0/api/notebook_get.md) request</span></span>

<span data-ttu-id="966ed-118">Os exemplos a seguir mostram como verificar o código de status da resposta, analisar o JSON para extrair as URLs e abrir o cliente do OneNote.</span><span class="sxs-lookup"><span data-stu-id="966ed-118">The following examples show how to check the status code of the response, parse the JSON to extract the URLs, and then open the OneNote client.</span></span>

## <a name="ios-example"></a><span data-ttu-id="966ed-119">Exemplo do iOS</span><span class="sxs-lookup"><span data-stu-id="966ed-119">iOS example</span></span>

<span data-ttu-id="966ed-120">O exemplo a seguir obtém as URLs de cliente do OneNote da resposta JSON.</span><span class="sxs-lookup"><span data-stu-id="966ed-120">The following example gets the OneNote client URLs from the JSON response.</span></span> <span data-ttu-id="966ed-121">Ele usa a biblioteca AFNetworking (http://afnetworking.com/) para extrair as duas URLs.</span><span class="sxs-lookup"><span data-stu-id="966ed-121">It uses the AFNetworking library (http://afnetworking.com/) to extract the two URLs.</span></span> <span data-ttu-id="966ed-122">No exemplo, `created` é um ponteiro para o objeto **ONSCPSStandardResponse** usado para armazenar os valores de resposta, e `responseObject` contém o JSON analisado.</span><span class="sxs-lookup"><span data-stu-id="966ed-122">In the example, `created` is a pointer to the ONSCPSStandardResponse object used to store the response values, and `responseObject` holds the parsed JSON.</span></span>

```objc
    /* Import the JSON library */
    #import "AFURLRequestSerialization.h"

    - (void)connectionDidFinishLoading:(NSURLConnection *)connection {
            if(delegate) {
                  int status = [returnResponse statusCode];
                  ONSCPSStandardResponse *standardResponse = nil;
                  if (status == 201) {
                        ONSCPSCreateSuccessResponse *created = 
                              [[ONSCPSCreateSuccessResponse alloc] init];
                        created.httpStatusCode = status;
                        NSError *jsonError;
                        NSDictionary *responseObject = 
                              [NSJSONSerialization JSONObjectWithData:returnData options:0 error:&jsonError];
                        if(responseObject && !jsonError) {
                              created.oneNoteClientUrl = ((NSDictionary *)
                                    ((NSDictionary *)responseObject[@"links"])[@"oneNoteClientUrl"])[@"href"];
                              created.oneNoteWebUrl = ((NSDictionary *)
                                    ((NSDictionary *)responseObject[@"links"])[@"oneNoteWebUrl"])[@"href"];
                        }
                  standardResponse = created;
                  }
                  else {
                        ONSCPSStandardErrorResponse *error = [[ONSCPSStandardErrorResponse alloc] init];
                        error.httpStatusCode = status;
                        error.message = [[NSString alloc] initWithData:returnData 
                              encoding:NSUTF8StringEncoding];
                        standardResponse = error;
                  }
                  // Send the response back to the client.
                  if (standardResponse) {
                        [delegate exampleServiceActionDidCompleteWithResponse: standardResponse];
                  }
            }
      }
``` 

<br/>

<span data-ttu-id="966ed-123">Após analisar as URLs de resposta, você poderá abrir o OneNote usando o código a seguir.</span><span class="sxs-lookup"><span data-stu-id="966ed-123">After you parse the URLs from the response, you can open OneNote by using the following code.</span></span> <span data-ttu-id="966ed-124">Use o `oneNoteClientUrl` para abrir o cliente do OneNote instalado ou o `oneNoteWebURL` para abrir o OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="966ed-124">Use `oneNoteClientUrl` to open the installed OneNote client or `oneNoteWebURL` to open OneNote Online.</span></span>

```objc
NSURL *url = [NSURL URLWithString:standardResponse.oneNoteWebUrl];
[[UIApplication sharedApplication] openURL:url];
```

## <a name="android-example"></a><span data-ttu-id="966ed-125">Exemplo do Android</span><span class="sxs-lookup"><span data-stu-id="966ed-125">Android example</span></span>

<span data-ttu-id="966ed-126">Primeiro, verifique se há o código de status de sucesso. Em seguida, analise o JSON.</span><span class="sxs-lookup"><span data-stu-id="966ed-126">First, check for the success status code and then parse the JSON.</span></span> <span data-ttu-id="966ed-127">O exemplo pressupõe que uma solicitação POST tenha sido enviada. Portanto, verifica se há um código de status `201 Created`.</span><span class="sxs-lookup"><span data-stu-id="966ed-127">The example assumes a POST request was sent, so it checks for a `201 Created` status code.</span></span> <span data-ttu-id="966ed-128">Se você tiver feito uma solicitação `GET`, verifique se há um código de status `200` em vez disso.</span><span class="sxs-lookup"><span data-stu-id="966ed-128">If you made a `GET` request, check for a `200` status code instead.</span></span>

```java
public ApiResponse getResponse() throws Exception {
    /* Get the HTTP response code and message from the connection object */
    int responseCode = mUrlConnection.getResponseCode();
    String responseMessage = mUrlConnection.getResponseMessage();
    String responseBody = null;

    /* Get the response if the new page was created successfully. */
    if ( responseCode == 201) {
        InputStream is = mUrlConnection.getInputStream();

        /* Verify that this byte array is big enough. */
        byte[] b1 = new byte[1024];
        StringBuffer buffer = new StringBuffer();

        /* Copy the body of the response into the new string. */
        /* Make sure the buffer is big enough. */
        while ( is.read(b1) != -1)
            buffer.append(new String(b1));

      /* When the returned data is complete, close the connection 
         and convert the byte array into a string. */
        mUrlConnection.disconnect();
        responseBody =  buffer.toString();
    }

    /* Create a new JSON object, and an object to hold the response URLs. */
    JSONObject responseObject = null;
    ApiResponse response = new ApiResponse();
    try {

        /* Store and verify the HTTP response code. */
        response.setResponseCode(responseCode);
        response.setResponseMessage(responseMessage);
        if ( responseCode == 201) {

            /* Retrieve the two URLs from the links property. */
            responseObject = new JSONObject(responseBody);
            String clientUrl = responseObject.getJSONObject(
                "links").getJSONObject("oneNoteClientUrl").getString("href");
            String webUrl = responseObject.getJSONObject(
                "links").getJSONObject("oneNoteWebUrl").getString("href");
            response.setOneNoteClientUrl(clientUrl);
            response.setOneNoteWebUrl(webUrl);
        }
    } catch (JSONException ex) {

        /* If the JSON was malformed or incomplete... */
        String msg = ex.getMessage();
        msg = msg;
    }
    return response;
}
```

<br/>

<span data-ttu-id="966ed-129">Usando as propriedades de resposta, o aplicativo pode abrir o OneNote Online, como mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="966ed-129">Using the response properties, your app can open OneNote Online, as shown in the following example.</span></span>

```java 
if (response.getResponseCode() == 201) {
    Uri uriUrl = Uri.parse(response.getOneNoteWebUrl);  
    Intent launchBrowser = new Intent(Intent.ACTION_VIEW, uriUrl); 
    startActivity(launchBrowser);
}
```

<br/>

<span data-ttu-id="966ed-130">Ou o aplicativo pode abrir o cliente do OneNote em um dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="966ed-130">Or your app can open the OneNote client on an Android device.</span></span> <span data-ttu-id="966ed-131">Ao usar a propriedade `oneNoteClientUrl`, você deve colocar as cadeias de caracteres de GUID entre chaves `{ }` antes de iniciar a Intenção.</span><span class="sxs-lookup"><span data-stu-id="966ed-131">When using the `oneNoteClientUrl` property, you must surround the GUID strings with braces `{ }` before starting the Intent.</span></span> <span data-ttu-id="966ed-132">O exemplo a seguir mostra como fazer isso.</span><span class="sxs-lookup"><span data-stu-id="966ed-132">The following example shows how to do that.</span></span>

```java 
if (response.getResponseCode() == 201) {

    // Get the URL from the OneNote API JSON response.
    String onenoteClientUrl = obtainClientLinkFromJSONResponse();
    String androidClientUrl = 
        onenoteClientUrl.replaceAll(
            "=([0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12})&",
            "={$1}&");

    // Open the URL: Open the newly created OneNote page.
    Uri uriUrl = Uri.parse(androidClientUrl);  
    Intent launchBrowser = new Intent(Intent.ACTION_VIEW, uriUrl); 
    startActivity(launchBrowser);
}
```

## <a name="see-also"></a><span data-ttu-id="966ed-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="966ed-133">See also</span></span>

- [<span data-ttu-id="966ed-134">Obter a estrutura e o conteúdo do OneNote</span><span class="sxs-lookup"><span data-stu-id="966ed-134">Get OneNote content and structure</span></span>](onenote-get-content.md)
- [<span data-ttu-id="966ed-135">Criar páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="966ed-135">Create OneNote pages</span></span>](onenote-create-page.md)