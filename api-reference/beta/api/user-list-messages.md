---
title: Listar mensagens
description: 'Obtenha as mensagens na caixa de correio do usuário conectado (incluindo as pastas Itens Excluídos e Email Secundário). '
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3a29392318de78c1e1ff5bd4ad4b560bc9c460f4
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2019
ms.locfileid: "31518529"
---
# <a name="list-messages"></a><span data-ttu-id="b8b81-103">Listar mensagens</span><span class="sxs-lookup"><span data-stu-id="b8b81-103">List messages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8b81-104">Obtenha as mensagens na caixa de correio do usuário conectado (incluindo as pastas Itens Excluídos e Email Secundário).</span><span class="sxs-lookup"><span data-stu-id="b8b81-104">Get the messages in the signed-in user's mailbox (including the Deleted Items and Clutter folders).</span></span> 

<span data-ttu-id="b8b81-105">Em particular, você pode filtrar as mensagens e obter apenas aquelas que incluem uma [menção](../resources/mention.md) do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="b8b81-105">In particular, you can filter on the messages and get only those that include a [mention](../resources/mention.md) of the signed-in user.</span></span>

<span data-ttu-id="b8b81-106">Observe que, por padrão, `GET /me/messages` a operação não retorna a propriedade **menciona** .</span><span class="sxs-lookup"><span data-stu-id="b8b81-106">Note that by default, the `GET /me/messages` operation does not return the **mentions** property.</span></span> <span data-ttu-id="b8b81-107">Use o `$expand` parâmetro de consulta para [encontrar detalhes de cada menção em uma mensagem](../api/message-get.md#request-2).</span><span class="sxs-lookup"><span data-stu-id="b8b81-107">Use the `$expand` query parameter to [find details of each mention in a message](../api/message-get.md#request-2).</span></span>

<span data-ttu-id="b8b81-108">Há dois cenários em que um aplicativo pode obter mensagens na pasta email de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="b8b81-108">There are two scenarios where an app can get messages in another user's mail folder:</span></span>

* <span data-ttu-id="b8b81-109">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="b8b81-109">If the app has application permissions, or,</span></span>
* <span data-ttu-id="b8b81-110">Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário, e outro usuário tiver compartilhado uma pasta de email com esse usuário, ou, o terá acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="b8b81-110">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="b8b81-111">Confira [detalhes e um exemplo](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="b8b81-111">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="b8b81-112">Permissões</span><span class="sxs-lookup"><span data-stu-id="b8b81-112">Permissions</span></span>
<span data-ttu-id="b8b81-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8b81-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8b81-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b8b81-115">Permission type</span></span>      | <span data-ttu-id="b8b81-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b8b81-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8b81-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b8b81-117">Delegated (work or school account)</span></span> | <span data-ttu-id="b8b81-118">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8b81-118">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b8b81-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b8b81-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8b81-120">Mail. ReadBasic, mail. Read, mail. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8b81-120">Mail.ReadBasic, Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="b8b81-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b8b81-121">Application</span></span> | <span data-ttu-id="b8b81-122">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8b81-122">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8b81-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b8b81-123">HTTP request</span></span>

<span data-ttu-id="b8b81-124">Para obter todas as mensagens na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="b8b81-124">To get all the messages in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages
GET /users/{id | userPrincipalName}/messages
```

<span data-ttu-id="b8b81-125">Para obter mensagens em uma pasta específica na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="b8b81-125">To get messages in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/messages
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages
```

<span data-ttu-id="b8b81-126">Para obter todas as mensagens na caixa de correio do usuário que incluam um **menção** do usuário:</span><span class="sxs-lookup"><span data-stu-id="b8b81-126">To get all the messages in the user's mailbox that include a **mention** of the user:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages?$filter=mentionsPreview/isMentioned eq true
GET /users/{id | userPrincipalName}/messages?$filter=mentionsPreview/isMentioned eq true
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b8b81-127">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b8b81-127">Optional query parameters</span></span>
<span data-ttu-id="b8b81-128">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="b8b81-128">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="b8b81-129">Você pode usar o `$filter` parâmetro de consulta na propriedade **mentionsPreview** para obter as mensagens que mencionam o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="b8b81-129">You can use the `$filter` query parameter on the **mentionsPreview** property to get those messages that mention the signed-in user.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8b81-130">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b8b81-130">Request headers</span></span>
| <span data-ttu-id="b8b81-131">Nome</span><span class="sxs-lookup"><span data-stu-id="b8b81-131">Name</span></span>       | <span data-ttu-id="b8b81-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8b81-132">Type</span></span> | <span data-ttu-id="b8b81-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8b81-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b8b81-134">Autorização</span><span class="sxs-lookup"><span data-stu-id="b8b81-134">Authorization</span></span>  | <span data-ttu-id="b8b81-135">string</span><span class="sxs-lookup"><span data-stu-id="b8b81-135">string</span></span>  | <span data-ttu-id="b8b81-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b8b81-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b8b81-138">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="b8b81-138">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="b8b81-139">string</span><span class="sxs-lookup"><span data-stu-id="b8b81-139">string</span></span> | <span data-ttu-id="b8b81-140">O formato das propriedades **body** e **uniqueBody** a serem retornadas.</span><span class="sxs-lookup"><span data-stu-id="b8b81-140">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="b8b81-141">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="b8b81-141">Values can be "text" or "html".</span></span> <span data-ttu-id="b8b81-142">Se o cabeçalho não for especificado, as propriedades **body** e **uniqueBody** serão retornadas no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="b8b81-142">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="b8b81-143">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b8b81-143">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8b81-144">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b8b81-144">Request body</span></span>
<span data-ttu-id="b8b81-145">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b8b81-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8b81-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="b8b81-146">Response</span></span>

<span data-ttu-id="b8b81-147">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [Message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8b81-147">If successful, this method returns a `200 OK` response code and collection of [message](../resources/message.md) objects in the response body.</span></span>

<span data-ttu-id="b8b81-148">O tamanho de página padrão para essa solicitação é dez mensagens.</span><span class="sxs-lookup"><span data-stu-id="b8b81-148">The default page size for this request is 10 messages.</span></span> 

## <a name="example"></a><span data-ttu-id="b8b81-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b8b81-149">Example</span></span>
##### <a name="request-1"></a><span data-ttu-id="b8b81-150">Solicitação 1</span><span class="sxs-lookup"><span data-stu-id="b8b81-150">Request 1</span></span>
<span data-ttu-id="b8b81-151">O primeiro exemplo obtém as 10 principais mensagens na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="b8b81-151">The first example gets the top 10 messages in the signed-in user's mailbox.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages
```
##### <a name="response-1"></a><span data-ttu-id="b8b81-152">Resposta 1</span><span class="sxs-lookup"><span data-stu-id="b8b81-152">Response 1</span></span>
<span data-ttu-id="b8b81-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8b81-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 317

{
  "value": [
    {
      "receivedDateTime": "2016-10-19T10:37:00Z",
      "sentDateTime": "2016-10-19T10:37:00Z",
      "hasAttachments": true,
      "subject": "subject-value",
      "body": {
        "contentType": "",
        "content": "content-value"
      },
      "bodyPreview": "bodyPreview-value"
    }
  ]
}
```


##### <a name="request-2"></a><span data-ttu-id="b8b81-156">Solicitação 2</span><span class="sxs-lookup"><span data-stu-id="b8b81-156">Request 2</span></span>
<span data-ttu-id="b8b81-157">O próximo exemplo filtra todas as mensagens na caixa de correio do usuário conectado para as que mencionam o usuário.</span><span class="sxs-lookup"><span data-stu-id="b8b81-157">The next example filters all messages in the signed-in user's mailbox for those that mention the user.</span></span> <span data-ttu-id="b8b81-158">Ele usa `$select` para retornar um subconjunto das propriedades de cada mensagem na resposta.</span><span class="sxs-lookup"><span data-stu-id="b8b81-158">It uses `$select` to return a subset of the properties of each message in the response.</span></span> 

<span data-ttu-id="b8b81-159">O exemplo também incorpora a codificação de URL para os caracteres de espaço na cadeia de caracteres de parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="b8b81-159">The example also incorporates URL encoding for the space characters in the query parameter string.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages_with_mentions"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$filter=MentionsPreview/IsMentioned%20eq%20true&$select=Subject,Sender,ReceivedDateTime,MentionsPreview
```
##### <a name="response-2"></a><span data-ttu-id="b8b81-160">Resposta 2</span><span class="sxs-lookup"><span data-stu-id="b8b81-160">Response 2</span></span>
<span data-ttu-id="b8b81-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b8b81-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 987

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#me/messages(subject,sender,receivedDateTime,mentionsPreview)",
  "value":[
    {
      "@odata.id":"https://graph.microsoft.com/beta/users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/messages('AQMkADJmMTUAAAgVZAAAA')",
      "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAATI\"",
      "id":"AQMkADJmMTUAAAgVZAAAA",
      "receivedDateTime":"2016-07-21T07:40:21Z",
      "subject":"Re: Start planning soon",
      "sender":{
        "emailAddress":{
          "name":"Randi Welch",
          "address":"randiw@contoso.onmicrosoft.com"
        }
      },
      "mentionsPreview":{
        "isMentioned":true
      }
    },
    {
      "@odata.id":"https://graph.microsoft.com/beta/Users('266efe5a-0fd7-4edd-877b-b2d1e561f193@ae01a323-3934-4475-a32d-af1274312bb0')/Messages('AQMkADJmMTUAAAjwVAAAA')",
      "@odata.etag":"W/\"CQAAABYAAAAPFhK2FclcRbABBJhCde8iAAAAAEGj\"",
      "id":"AQMkADJmMTUAAAjwVAAAA",
      "receivedDateTime":"2016-07-21T07:40:20Z",
      "subject":"Re: Start planning soon",
      "sender":{
        "emailAddress":{
          "name":"Randi Welch",
          "address":"randiw@contoso.onmicrosoft.com"
        }
      },
      "mentionsPreview":{
        "isMentioned":true
      }
    }
  ]
}
```

##### <a name="request-3"></a><span data-ttu-id="b8b81-164">Solicitação 3</span><span class="sxs-lookup"><span data-stu-id="b8b81-164">Request 3</span></span>
<span data-ttu-id="b8b81-165">O terceiro exemplo mostra como usar um `Prefer: outlook.body-content-type="text"` cabeçalho para obter as propriedades **Body** e **uniqueBody** de cada mensagem em formato de texto.</span><span class="sxs-lookup"><span data-stu-id="b8b81-165">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** properties of each message in text format.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_messages_in_text"
}-->
```http
GET https://graph.microsoft.com/beta/me/messages?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
##### <a name="response-3"></a><span data-ttu-id="b8b81-166">Resposta 3</span><span class="sxs-lookup"><span data-stu-id="b8b81-166">Response 3</span></span>
<span data-ttu-id="b8b81-167">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b8b81-167">Here is an example of the response.</span></span> 

<!--
Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.
-->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2704

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('cd209b0b-3f83-4c35-82d2-d88a61820480')/messages(subject,body,bodyPreview,uniqueBody)",
    "value":[
        {
            "@odata.type":"#microsoft.graph.eventMessageRequest",
            "@odata.etag":"W/\"CwAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj5\"",
            "id":"AAMkAGIAAAoZCfIAAA=",
            "subject":"Orientation ",
            "bodyPreview":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.",
            "body":{
                "contentType":"text",
                "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Dana, this is the time you selected for our orientation. Please bring the notes I sent you.\r\n"
            }
        },
        {
            "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAoZYj4\"",
            "id":"AAMkAGIAAAoZCfHAAA=",
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
        },
        {
            "@odata.etag":"W/\"CQAAABYAAABmWdbhEgBXTophjCWt81m9AAAAAAjr\"",
            "id":"AQMkAGIAAAIJTQAAAA==",
            "subject":"Welcome aboard!",
            "bodyPreview":"Welcome to the Support group!",
            "body":{
                "contentType":"text",
                "content":"Welcome to the Support group!\r\n"
            },
            "uniqueBody":{
                "contentType":"text",
                "content":"Welcome to the Support group!\r\n"
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-messages.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
