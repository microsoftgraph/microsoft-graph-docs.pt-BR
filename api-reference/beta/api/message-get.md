---
title: Obter mensagem
description: Recupere as propriedades e os relacionamentos do objeto Message.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 8d15a1f07ae42e9c203a26a970896fea0d360494
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31518515"
---
# <a name="get-message"></a><span data-ttu-id="c7f9a-103">Obter mensagem</span><span class="sxs-lookup"><span data-stu-id="c7f9a-103">Get message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7f9a-104">Recupere as propriedades e os relacionamentos do objeto [Message](../resources/message.md) .</span><span class="sxs-lookup"><span data-stu-id="c7f9a-104">Retrieve the properties and relationships of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="c7f9a-105">Por exemplo, você pode obter uma mensagem e expandir todas as instâncias de [menção](../resources/mention.md) na mensagem.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-105">For example, you can get a message and expand all the [mention](../resources/mention.md) instances in the message.</span></span>

<span data-ttu-id="c7f9a-106">Há dois cenários em que um aplicativo pode obter uma mensagem na pasta email de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="c7f9a-106">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="c7f9a-107">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="c7f9a-107">If the app has application permissions, or,</span></span>
* <span data-ttu-id="c7f9a-108">Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário, e outro usuário tiver compartilhado uma pasta de email com esse usuário, ou, o terá acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-108">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="c7f9a-109">Confira [detalhes e um exemplo](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="c7f9a-109">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="c7f9a-110">Como o recurso **message** dá suporte a [extensions](/graph/extensibility-overview), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **message**.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-110">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="c7f9a-111">Permissões</span><span class="sxs-lookup"><span data-stu-id="c7f9a-111">Permissions</span></span>
<span data-ttu-id="c7f9a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7f9a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7f9a-114">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c7f9a-114">Permission type</span></span>      | <span data-ttu-id="c7f9a-115">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c7f9a-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7f9a-116">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c7f9a-116">Delegated (work or school account)</span></span> | <span data-ttu-id="c7f9a-117">Mail. ReadBasic, mail. Read</span><span class="sxs-lookup"><span data-stu-id="c7f9a-117">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="c7f9a-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c7f9a-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7f9a-119">Mail. ReadBasic, mail. Read</span><span class="sxs-lookup"><span data-stu-id="c7f9a-119">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="c7f9a-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c7f9a-120">Application</span></span> | <span data-ttu-id="c7f9a-121">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c7f9a-121">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7f9a-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c7f9a-122">HTTP request</span></span>

<span data-ttu-id="c7f9a-123">Para obter a mensagem especificada:</span><span class="sxs-lookup"><span data-stu-id="c7f9a-123">To get the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="c7f9a-124">Para obter uma mensagem e expandir todas as menção na mensagem:</span><span class="sxs-lookup"><span data-stu-id="c7f9a-124">To get a message and expand all mentions in the message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/messages/{id}?$expand=mentions
GET /me/mailFolders/{id}/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}?$expand=mentions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7f9a-125">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c7f9a-125">Optional query parameters</span></span>
<span data-ttu-id="c7f9a-126">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="c7f9a-127">Você pode usar o `$expand` parâmetro de consulta na propriedade de navegação **menciona** para obter uma mensagem com os detalhes de cada [menção](../resources/mention.md) na mensagem expandida.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-127">You can use the `$expand` query parameter on the **mentions** navigation property to get a message with the details of each [mention](../resources/mention.md) in the message expanded.</span></span>



## <a name="request-headers"></a><span data-ttu-id="c7f9a-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c7f9a-128">Request headers</span></span>
| <span data-ttu-id="c7f9a-129">Nome</span><span class="sxs-lookup"><span data-stu-id="c7f9a-129">Name</span></span>       | <span data-ttu-id="c7f9a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7f9a-130">Type</span></span> | <span data-ttu-id="c7f9a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7f9a-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c7f9a-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="c7f9a-132">Authorization</span></span>  | <span data-ttu-id="c7f9a-133">string</span><span class="sxs-lookup"><span data-stu-id="c7f9a-133">string</span></span>  | <span data-ttu-id="c7f9a-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c7f9a-136">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="c7f9a-136">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="c7f9a-137">string</span><span class="sxs-lookup"><span data-stu-id="c7f9a-137">string</span></span> | <span data-ttu-id="c7f9a-138">O formato das propriedades **body** e **uniqueBody** a serem retornadas.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-138">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="c7f9a-139">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="c7f9a-139">Values can be "text" or "html".</span></span> <span data-ttu-id="c7f9a-140">Um cabeçalho `Preference-Applied` é retornado como confirmação quando este cabeçalho `Prefer` é especificado.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-140">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="c7f9a-141">Se o cabeçalho não for especificado, as propriedades **body** e **uniqueBody** serão retornadas no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-141">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="c7f9a-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-142">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7f9a-143">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c7f9a-143">Request body</span></span>
<span data-ttu-id="c7f9a-144">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7f9a-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="c7f9a-145">Response</span></span>

<span data-ttu-id="c7f9a-146">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-146">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c7f9a-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c7f9a-147">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="c7f9a-148">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="c7f9a-148">Request 1</span></span>
<span data-ttu-id="c7f9a-149">O primeiro exemplo obtém a mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-149">The first example gets the specified message.</span></span> <span data-ttu-id="c7f9a-150">Ele não especifica nenhum cabeçalho para indicar o formato desejado do corpo a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-150">It does not specify any header to indicate the desired format of the body to be returned.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGI1AAAoZCfHAAA=')
```
##### <a name="response-1"></a><span data-ttu-id="c7f9a-151">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="c7f9a-151">Response 1</span></span>
<span data-ttu-id="c7f9a-152">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-152">Here is an example of the response.</span></span> <span data-ttu-id="c7f9a-153">As propriedades **Body** e **uniqueBody** são retornadas no formato HTML padrão.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-153">The **body** and **uniqueBody** properties are returned in the default HTML format.</span></span>
<span data-ttu-id="c7f9a-154">Observação: o objeto Response mostrado aqui é truncado por brevidade.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-154">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="c7f9a-155">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-155">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 523

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/messages/$entity",
    "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj4\"",
    "id":"AAMkAGI1AAAoZCfHAAA=",
    "subject":"Welcome to our group!",
    "bodyPreview":"Welcome to our group, Dana! Hope you will enjoy working with us !\r\n",
    "body":{
        "contentType":"html",
        "content":"<html>\r\n<head></head><body><p>Welcome to our group, Dana! Hope you will enjoy working with us </p></body></html>\r\n"
    },
    "uniqueBody":{
        "contentType":"html",
        "content":"<html>\r\n<head></head><body><p>Welcome to our group, Dana! Hope you will enjoy working with us </p></body></html>\r\n"
    }
}
```

##### <a name="request-2"></a><span data-ttu-id="c7f9a-156">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="c7f9a-156">Request 2</span></span>
<span data-ttu-id="c7f9a-157">No próximo exemplo, o usuário conectado é Dana Swope.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-157">In the next example, the signed-in user is Dana Swope.</span></span> <span data-ttu-id="c7f9a-158">O exemplo mostra a obtenção de detalhes de todas as menções na mensagem especificada na caixa de correio da Dana.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-158">The example shows getting the details of all the mentions in the specified message in Dana's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADJmMTUAAAgVZAAAA"],
  "name": "get_mentions_in_message"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages/('AQMkADJmMTUAAAgVZAAAA')?$expand=mentions
```
##### <a name="response-2"></a><span data-ttu-id="c7f9a-159">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="c7f9a-159">Response 2</span></span>
<span data-ttu-id="c7f9a-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2248

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages/$entity",
  "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')",
  "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAATI\"",
  "id":"AQMkADJmMTUAAAgVZAAAA",
  "subject":"Start planning soon",
  "body":{
    "contentType":"HTML",
    "content":"<html><head></head><body><p><a href=\"mailto:danas@contoso.onmicrosoft.com\">@Dana Swope</a>,<a href=\"mailto:randiw@contoso.onmicrosoft.com\">@Randi Welch</a>, forgot to mention, I will be away&nbsp;this weekend. I can start on Monday though.</p></body></html>"
  },
  "bodyPreview":"@Dana Swope<mailto:danas@contoso.onmicrosoft.com>, @Randi Welch, forgot to mention, I will be away this weekend. I can start on Monday though.",
  "sender":{
    "emailAddress":{
      "name":"Samantha Booth",
      "address":"samanthab@contoso.onmicrosoft.com"
    }
  },
  "from":{
    "emailAddress":{
      "name":"Samantha Booth",
      "address":"samanthab@contoso.onmicrosoft.com"
    }
  },
  "toRecipients":[
    {
      "emailAddress":{
        "name":"Dana Swope",
        "address":"danas@contoso.onmicrosoft.com"
      }
    },
    {
      "emailAddress":{
        "name":"Randi Welch",
        "address":"randiw@contoso.onmicrosoft.com"
      }
    }
  ],
  "ccRecipients":[
  ],
  "bccRecipients":[
  ],
  "mentionsPreview":{
    "isMentioned":true
  },
  "mentions@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages('AQMkADJmMTUAAAgVZAAAA')/mentions",
  "mentions":[
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')/mentions('138f4c0a-1130-4776-b780-bf79d73abb3f')",
      "id":"138f4c0a-1130-4776-b780-bf79d73abb3f",
      "mentioned":{
        "name":"Dana Swope",
        "address":"danas@contoso.onmicrosoft.com"
      },
      "mentionText":null,
      "clientReference":null,
      "createdBy":{
        "name":"Samantha Booth",
        "address":"samanthab@contoso.onmicrosoft.com"
      },
      "createdDateTime":"2016-07-21T07:40:20.152Z",
      "serverCreatedDateTime":"2016-07-21T07:40:20.152Z",
      "deepLink":null,
      "application":null
    },
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')/mentions('7b94df1a-0086-482a-b0da-e62fae12f983')",
      "id":"7b94df1a-0086-482a-b0da-e62fae12f983",
      "mentioned":{
        "name":"Randi Welch",
        "address":"randiw@contoso.onmicrosoft.com"
      },
      "mentionText":null,
      "clientReference":null,
      "createdBy":{
        "name":"Samantha Booth",
        "address":"samanthab@contoso.onmicrosoft.com"
      },
      "createdDateTime":"2016-07-21T07:40:20.158Z",
      "serverCreatedDateTime":"2016-07-21T07:40:20.158Z",
      "deepLink":null,
      "application":null
    }
  ]
}
```


##### <a name="request-3"></a><span data-ttu-id="c7f9a-163">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="c7f9a-163">Request 3</span></span>

<span data-ttu-id="c7f9a-164">O terceiro exemplo mostra como usar um `Prefer: outlook.body-content-type="text"` cabeçalho para obter o **corpo** e **uniqueBody** da mensagem especificada no formato de texto.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-164">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** of the specified message in text format.</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message_in_text"
}-->

```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGI1AAAoZCfHAAA=')?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```

##### <a name="response-3"></a><span data-ttu-id="c7f9a-165">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="c7f9a-165">Response 3</span></span>

<span data-ttu-id="c7f9a-166">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-166">Here is an example of the response.</span></span> <span data-ttu-id="c7f9a-167">Observação: a resposta inclui um `Preference-Applied: outlook.body-content-type` cabeçalho para confirmar o `Prefer: outlook.body-content-type` cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-167">Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.body-content-type="text"
Content-length: 1550

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/messages(subject,body,bodyPreview,uniqueBody)/$entity",
    "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj4\"",
    "id":"AAMkAGI1AAAoZCfHAAA=",
    "subject":"Welcome to our group!",
    "bodyPreview":"Welcome to our group, Dana! Hope you will enjoy working with us !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nTh",
    "body":{
        "contentType":"text",
        "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\n\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\n\r\nThanks!\r\n\r\n"
    },
    "uniqueBody":{
        "contentType":"text",
        "content":"Welcome to our group, Dana! Hope you will enjoy working with us [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] [\ud83d\ude0a] !\r\nWould you like to choose a day for our orientation from the available times below:\r\n\r\nDate\r\n        Time\r\n\r\nApril 14, 2017\r\n        1-3pm\r\n\r\nApril 21, 2017\r\n        10-12noon\r\n\r\n\r\nThanks!\r\n"
    }
}
```

##### <a name="request-4"></a><span data-ttu-id="c7f9a-168">Solicitação 4</span><span class="sxs-lookup"><span data-stu-id="c7f9a-168">Request 4</span></span>

<span data-ttu-id="c7f9a-169">O quarto exemplo mostra como obter os cabeçalhos de mensagem da Internet de uma mensagem específica.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-169">The fourth example shows how to get the Internet message headers of a specific message.</span></span>  

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEz"],
  "name": "get_message_internet_headers"
}-->

```http
GET https://graph.microsoft.com/beta/me/messages('AAMkAGVmMDEz')?$select=internetMessageHeaders
```

##### <a name="response-4"></a><span data-ttu-id="c7f9a-170">Resposta 4</span><span class="sxs-lookup"><span data-stu-id="c7f9a-170">Response 4</span></span>

<span data-ttu-id="c7f9a-171">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-171">Here is an example of the response.</span></span> <span data-ttu-id="c7f9a-172">Observação: o número de cabeçalhos de mensagens da Internet no objeto Response foi reduzido por brevidade.</span><span class="sxs-lookup"><span data-stu-id="c7f9a-172">Note: The number of Internet message headers in the response object has been reduced for brevity.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('48d31887-5fad-4d73-a9f5-3c356e68a038')/messages(internetMessageHeaders)/$entity",
  "@odata.type":"#microsoft.graph.eventMessageRequest",
  "@odata.etag":"W/\"CwAAABYAAAAiIsqMbYjsT5e/T7KzowPTAAAa/qUB\"",
  "id":"AAMkAGVmMDEz",
  "internetMessageHeaders":[
    {
      "name":"Content-Type",
      "value":"application/ms-tnef"
    },
    {
      "name":"Content-Transfer-Encoding",
      "value":"binary"
    },
    {
      "name":"Subject",
      "value":"Cloud and Mobile Working Group"
    },
    {
      "name":"x-custom-header-group-name",
      "value":"Washington"
    },
    {
      "name":"x-custom-header-group-id",
      "value":"WA001"
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="c7f9a-173">Confira também</span><span class="sxs-lookup"><span data-stu-id="c7f9a-173">See also</span></span>

- [<span data-ttu-id="c7f9a-174">Adicionar dados personalizados aos recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="c7f9a-174">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="c7f9a-175">Adicionar dados personalizados aos usuários usando extensões abertas (visualização)</span><span class="sxs-lookup"><span data-stu-id="c7f9a-175">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="c7f9a-176">Adicionar dados personalizados a grupos usando extensões de esquema (visualização)</span><span class="sxs-lookup"><span data-stu-id="c7f9a-176">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
