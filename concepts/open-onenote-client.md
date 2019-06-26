---
title: abrir o cliente do OneNote
description: 'Você pode usar a propriedade **links** de uma página ou de um bloco de anotações para abrir um aplicativo do OneNote em determinada página ou bloco de anotações. '
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: b4ad078443bd6d85c46a6e23552ddc730c725b51
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236283"
---
# <a name="open-the-onenote-client"></a><span data-ttu-id="f9eb8-103">Abrir o cliente do OneNote</span><span class="sxs-lookup"><span data-stu-id="f9eb8-103">Open the OneNote client</span></span>

<span data-ttu-id="f9eb8-104">Você pode usar a propriedade **links** de uma página ou de um bloco de anotações para abrir um aplicativo do OneNote em determinada página ou bloco de anotações.</span><span class="sxs-lookup"><span data-stu-id="f9eb8-104">You can use the **links** property of a page or notebook to open a OneNote application to a particular page or notebook.</span></span> 

<span data-ttu-id="f9eb8-105">A propriedade **links** é um objeto JSON que contém duas URLs.</span><span class="sxs-lookup"><span data-stu-id="f9eb8-105">The **links** property is a JSON object that contains two URLs.</span></span> <span data-ttu-id="f9eb8-106">As URLs abrirão a página ou o bloco de anotações no aplicativo cliente do OneNote ou no OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="f9eb8-106">The URLs will open the page or notebook in the OneNote client application or in OneNote on the web.</span></span>

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

- <span data-ttu-id="f9eb8-107">**oneNoteClientUrl**</span><span class="sxs-lookup"><span data-stu-id="f9eb8-107">**oneNoteClientUrl**</span></span> 

    - <span data-ttu-id="f9eb8-108">Abre o cliente do OneNote, caso já esteja instalado no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9eb8-108">Opens the OneNote client if it is already installed on the device.</span></span> <span data-ttu-id="f9eb8-109">Essa URL inclui o prefixo *onenote*.</span><span class="sxs-lookup"><span data-stu-id="f9eb8-109">This URL includes the *onenote* prefix.</span></span>
    - <span data-ttu-id="f9eb8-110">Abre a versão de idioma específico, caso esteja instalada no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f9eb8-110">Opens the language-specific version if one is installed on the device.</span></span> <span data-ttu-id="f9eb8-111">Caso contrário, usa a configuração de idioma da plataforma.</span><span class="sxs-lookup"><span data-stu-id="f9eb8-111">Otherwise, uses the platform language setting.</span></span>

- <span data-ttu-id="f9eb8-112">**oneNoteWebUrl**</span><span class="sxs-lookup"><span data-stu-id="f9eb8-112">**oneNoteWebUrl**</span></span> 

    - <span data-ttu-id="f9eb8-113">Abre o OneNote na Web se o navegador padrão no dispositivo oferecer suporte a ele.</span><span class="sxs-lookup"><span data-stu-id="f9eb8-113">Opens OneNote on the web if the default browser on the device supports it.</span></span> 
    - <span data-ttu-id="f9eb8-114">Usa a configuração de idioma do navegador.</span><span class="sxs-lookup"><span data-stu-id="f9eb8-114">Uses the browser language setting.</span></span>


<span data-ttu-id="f9eb8-115">A API do OneNote retorna a propriedade **links** na resposta HTTP para as seguintes operações:</span><span class="sxs-lookup"><span data-stu-id="f9eb8-115">The OneNote API returns the **links** property in the HTTP response for the following operations:</span></span>

- <span data-ttu-id="f9eb8-116">Crie uma página enviando uma solicitação [`POST pages`](/graph/api/section-post-pages?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="f9eb8-116">Create a page by sending a [`POST pages`](/graph/api/section-post-pages?view=graph-rest-1.0) request.</span></span>

- <span data-ttu-id="f9eb8-117">Crie um bloco de anotações enviando uma solicitação [`POST notebooks`](/graph/api/onenote-post-notebooks?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="f9eb8-117">Create a notebook by sending a [`POST notebooks`](/graph/api/onenote-post-notebooks?view=graph-rest-1.0) request.</span></span>

- <span data-ttu-id="f9eb8-118">Obtenha os metadados de página enviando uma solicitação [`GET pages`](/graph/api/page-get?view=graph-rest-1.0) ou [`GET pages/{id}`](/graph/api/page-get?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="f9eb8-118">Get page metadata by sending a [`GET pages`](/graph/api/page-get?view=graph-rest-1.0) or [`GET pages/{id}`](/graph/api/page-get?view=graph-rest-1.0) request.</span></span>

- <span data-ttu-id="f9eb8-119">Obtenha metadados de bloco de anotações enviando uma solicitação [`GET notebooks`](/graph/api/notebook-get?view=graph-rest-1.0) ou [`GET notebooks/{id}`](/graph/api/notebook-get?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="f9eb8-119">Get notebook metadata by sending a [`GET notebooks`](/graph/api/notebook-get?view=graph-rest-1.0) or [`GET notebooks/{id}`](/graph/api/notebook-get?view=graph-rest-1.0) request.</span></span>

<span data-ttu-id="f9eb8-120">Os exemplos a seguir mostram como verificar o código de status da resposta, analisar o JSON para extrair as URLs e abrir o cliente do OneNote.</span><span class="sxs-lookup"><span data-stu-id="f9eb8-120">The following examples show how to check the status code of the response, parse the JSON to extract the URLs, and then open the OneNote client.</span></span>

## <a name="ios-example"></a><span data-ttu-id="f9eb8-121">Exemplo do iOS</span><span class="sxs-lookup"><span data-stu-id="f9eb8-121">iOS example</span></span>

<span data-ttu-id="f9eb8-122">O exemplo a seguir obtém as URLs de cliente do OneNote da resposta JSON.</span><span class="sxs-lookup"><span data-stu-id="f9eb8-122">The following example gets the OneNote client URLs from the JSON response.</span></span> <span data-ttu-id="f9eb8-123">Ele usa a biblioteca AFNetworking (https://afnetworking.com/) para extrair as duas URLs.</span><span class="sxs-lookup"><span data-stu-id="f9eb8-123">It uses the AFNetworking library (https://afnetworking.com/) to extract the two URLs.</span></span> <span data-ttu-id="f9eb8-124">No exemplo, `created` é um ponteiro para o objeto **ONSCPSStandardResponse** usado para armazenar os valores de resposta, e `responseObject` contém o JSON analisado.</span><span class="sxs-lookup"><span data-stu-id="f9eb8-124">In the example, `created` is a pointer to the **ONSCPSStandardResponse** object used to store the response values, and `responseObject` holds the parsed JSON.</span></span>

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

<span data-ttu-id="f9eb8-125">Após analisar as URLs de resposta, você poderá abrir o OneNote usando o código a seguir.</span><span class="sxs-lookup"><span data-stu-id="f9eb8-125">After you parse the URLs from the response, you can open OneNote by using the following code.</span></span> <span data-ttu-id="f9eb8-126">Use `oneNoteClientUrl` o para abrir o cliente do OneNote `oneNoteWebURL` instalado ou para abrir o OneNote na Web.</span><span class="sxs-lookup"><span data-stu-id="f9eb8-126">Use `oneNoteClientUrl` to open the installed OneNote client or `oneNoteWebURL` to open OneNote on the web.</span></span>

```objc
NSURL *url = [NSURL URLWithString:standardResponse.oneNoteWebUrl];
[[UIApplication sharedApplication] openURL:url];
```

## <a name="android-example"></a><span data-ttu-id="f9eb8-127">Exemplo do Android</span><span class="sxs-lookup"><span data-stu-id="f9eb8-127">Android example</span></span>

<span data-ttu-id="f9eb8-128">Primeiro, verifique se há o código de status de sucesso. Em seguida, analise o JSON.</span><span class="sxs-lookup"><span data-stu-id="f9eb8-128">First, check for the success status code, and then parse the JSON.</span></span> <span data-ttu-id="f9eb8-129">O exemplo pressupõe que uma solicitação POST tenha sido enviada. Portanto, verifica se há um código de status `201 Created`.</span><span class="sxs-lookup"><span data-stu-id="f9eb8-129">The example assumes a POST request was sent, so it checks for a `201 Created` status code.</span></span> <span data-ttu-id="f9eb8-130">Se você tiver feito uma solicitação `GET`, verifique se há um código de status `200` em vez disso.</span><span class="sxs-lookup"><span data-stu-id="f9eb8-130">If you made a `GET` request, check for a `200` status code instead.</span></span>

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

<span data-ttu-id="f9eb8-131">Usando as propriedades de resposta, seu aplicativo pode abrir o OneNote na Web, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="f9eb8-131">Using the response properties, your app can open OneNote on the web, as shown in the following example.</span></span>

```java 
if (response.getResponseCode() == 201) {
    Uri uriUrl = Uri.parse(response.getOneNoteWebUrl);  
    Intent launchBrowser = new Intent(Intent.ACTION_VIEW, uriUrl); 
    startActivity(launchBrowser);
}
```

<br/>

<span data-ttu-id="f9eb8-132">Ou o aplicativo pode abrir o cliente do OneNote em um dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="f9eb8-132">Or your app can open the OneNote client on an Android device.</span></span> <span data-ttu-id="f9eb8-133">Ao usar a propriedade `oneNoteClientUrl`, você deve colocar as cadeias de caracteres de GUID entre chaves `{ }` antes de iniciar a Intenção.</span><span class="sxs-lookup"><span data-stu-id="f9eb8-133">When using the `oneNoteClientUrl` property, you must surround the GUID strings with braces `{ }` before starting the Intent.</span></span> <span data-ttu-id="f9eb8-134">O exemplo a seguir mostra como fazer isso.</span><span class="sxs-lookup"><span data-stu-id="f9eb8-134">The following example shows how to do that.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="f9eb8-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="f9eb8-135">See also</span></span>

- [<span data-ttu-id="f9eb8-136">Obter a estrutura e o conteúdo do OneNote</span><span class="sxs-lookup"><span data-stu-id="f9eb8-136">Get OneNote content and structure</span></span>](onenote-get-content.md)
- [<span data-ttu-id="f9eb8-137">Criar páginas do OneNote</span><span class="sxs-lookup"><span data-stu-id="f9eb8-137">Create OneNote pages</span></span>](onenote-create-page.md)
