---
title: abrir o cliente do OneNote
description: 'Você pode usar a propriedade **links** de uma página ou de um bloco de anotações para abrir um aplicativo do OneNote em determinada página ou bloco de anotações. '
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: ada371ab457e4bd5c760770dbdc2baaea8557efeef14a5fe1ddb37c2f4c33059
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54123902"
---
# <a name="open-the-onenote-client"></a>Abrir o cliente do OneNote

Você pode usar a propriedade **links** de uma página ou de um bloco de anotações para abrir um aplicativo do OneNote em determinada página ou bloco de anotações. 

A propriedade **links** é um objeto JSON que contém duas URLs. As URLs abrirão a página ou bloco de anotações no aplicativo OneNote cliente ou no OneNote na Web.

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

- **oneNoteClientUrl** 

  - Abre o cliente do OneNote, caso já esteja instalado no dispositivo. Essa URL inclui o prefixo *onenote*.
  - Abre a versão de idioma específico, caso esteja instalada no dispositivo. Caso contrário, usa a configuração de idioma da plataforma.

- **oneNoteWebUrl** 

  - Abre OneNote na Web se o navegador padrão no dispositivo oferece suporte a ele. 
  - Usa a configuração de idioma do navegador.


A API do OneNote retorna a propriedade **links** na resposta HTTP para as seguintes operações:

- Crie uma página enviando uma solicitação [`POST pages`](/graph/api/section-post-pages?view=graph-rest-1.0).

- Crie um bloco de anotações enviando uma solicitação [`POST notebooks`](/graph/api/onenote-post-notebooks?view=graph-rest-1.0).

- Obtenha os metadados de página enviando uma solicitação [`GET pages`](/graph/api/page-get?view=graph-rest-1.0) ou [`GET pages/{id}`](/graph/api/page-get?view=graph-rest-1.0).

- Obtenha metadados de bloco de anotações enviando uma solicitação [`GET notebooks`](/graph/api/notebook-get?view=graph-rest-1.0) ou [`GET notebooks/{id}`](/graph/api/notebook-get?view=graph-rest-1.0).

Os exemplos a seguir mostram como verificar o código de status da resposta, analisar o JSON para extrair as URLs e abrir o cliente do OneNote.

## <a name="ios-example"></a>Exemplo do iOS

O exemplo a seguir obtém as URLs de cliente do OneNote da resposta JSON. Ele usa a biblioteca AFNetworking (https://afnetworking.com/) para extrair as duas URLs. No exemplo, `created` é um ponteiro para o objeto **ONSCPSStandardResponse** usado para armazenar os valores de resposta, e `responseObject` contém o JSON analisado.

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

Após analisar as URLs de resposta, você poderá abrir o OneNote usando o código a seguir. Use `oneNoteClientUrl` para abrir o cliente OneNote instalado ou para abrir `oneNoteWebURL` OneNote na Web.

```objc
NSURL *url = [NSURL URLWithString:standardResponse.oneNoteWebUrl];
[[UIApplication sharedApplication] openURL:url];
```

## <a name="android-example"></a>Exemplo do Android

Primeiro, verifique se há o código de status de sucesso. Em seguida, analise o JSON. O exemplo pressupõe que uma solicitação POST tenha sido enviada. Portanto, verifica se há um código de status `201 Created`. Se você tiver feito uma solicitação `GET`, verifique se há um código de status `200` em vez disso.

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

Usando as propriedades de resposta, seu aplicativo pode OneNote na Web, conforme mostrado no exemplo a seguir.

```java 
if (response.getResponseCode() == 201) {
    Uri uriUrl = Uri.parse(response.getOneNoteWebUrl);  
    Intent launchBrowser = new Intent(Intent.ACTION_VIEW, uriUrl); 
    startActivity(launchBrowser);
}
```

<br/>

Ou o aplicativo pode abrir o cliente do OneNote em um dispositivo Android. Ao usar a propriedade `oneNoteClientUrl`, você deve colocar as cadeias de caracteres de GUID entre chaves `{ }` antes de iniciar a Intenção. O exemplo a seguir mostra como fazer isso.

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

## <a name="see-also"></a>Confira também

- [Obter a estrutura e o conteúdo do OneNote](onenote-get-content.md)
- [Criar páginas do OneNote](onenote-create-page.md)
