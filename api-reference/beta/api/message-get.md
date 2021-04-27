---
title: Obter mensagem
description: Recupere as propriedades e as relações do objeto message.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: a727179016a5352a55d0923dfcd5ac5834f73d84
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050154"
---
# <a name="get-message"></a><span data-ttu-id="a973a-103">Obter mensagem</span><span class="sxs-lookup"><span data-stu-id="a973a-103">Get message</span></span>

<span data-ttu-id="a973a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a973a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a973a-105">Recupere as propriedades e as relações do [objeto message.](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="a973a-105">Retrieve the properties and relationships of the [message](../resources/message.md) object.</span></span>

<span data-ttu-id="a973a-106">Por exemplo, você pode obter uma mensagem e expandir todas [as](../resources/mention.md) instâncias de menção na mensagem.</span><span class="sxs-lookup"><span data-stu-id="a973a-106">For instance, you can get a message and expand all the [mention](../resources/mention.md) instances in the message.</span></span> <span data-ttu-id="a973a-107">Veja um [exemplo](#example-2-get-all-mentions-in-a-specific-message) abaixo.</span><span class="sxs-lookup"><span data-stu-id="a973a-107">See an [example](#example-2-get-all-mentions-in-a-specific-message) below.</span></span>

<span data-ttu-id="a973a-108">Você pode usar o `$value` parâmetro para [obter o conteúdo MIME de uma mensagem](/graph/outlook-get-mime-message).</span><span class="sxs-lookup"><span data-stu-id="a973a-108">You can use the `$value` parameter to [get the MIME content of a message](/graph/outlook-get-mime-message).</span></span> <span data-ttu-id="a973a-109">Veja também um [exemplo](#example-5-get-mime-content) abaixo.</span><span class="sxs-lookup"><span data-stu-id="a973a-109">See also an [example](#example-5-get-mime-content) below.</span></span>

<span data-ttu-id="a973a-110">Existem dois cenários em que um aplicativo pode receber mensagens na pasta de email de outro usuário:</span><span class="sxs-lookup"><span data-stu-id="a973a-110">There are two scenarios where an app can get a message in another user's mail folder:</span></span>

* <span data-ttu-id="a973a-111">Se o aplicativo tiver permissões de aplicativo ou</span><span class="sxs-lookup"><span data-stu-id="a973a-111">If the app has application permissions, or,</span></span>
* <span data-ttu-id="a973a-112">Se o aplicativo tiver as [permissões](#permissions) delegadas apropriadas de um usuário e outro usuário tiver compartilhado uma pasta de email com esse usuário, ou tiver concedido acesso delegado a esse usuário.</span><span class="sxs-lookup"><span data-stu-id="a973a-112">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="a973a-113">Confira [detalhes e um exemplo](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="a973a-113">See [details and an example](/graph/outlook-share-messages-folders).</span></span>

<span data-ttu-id="a973a-114">Como o recurso **message** dá suporte a [extensions](/graph/extensibility-overview), você também pode usar a operação `GET` para obter propriedades personalizadas e dados de extensão em uma instância de **message**.</span><span class="sxs-lookup"><span data-stu-id="a973a-114">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **message** instance.</span></span>


## <a name="permissions"></a><span data-ttu-id="a973a-115">Permissões</span><span class="sxs-lookup"><span data-stu-id="a973a-115">Permissions</span></span>
<span data-ttu-id="a973a-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a973a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a973a-118">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a973a-118">Permission type</span></span>      | <span data-ttu-id="a973a-119">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a973a-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a973a-120">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a973a-120">Delegated (work or school account)</span></span> | <span data-ttu-id="a973a-121">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a973a-121">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="a973a-122">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a973a-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a973a-123">Mail.ReadBasic, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a973a-123">Mail.ReadBasic, Mail.Read</span></span>    |
|<span data-ttu-id="a973a-124">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a973a-124">Application</span></span> | <span data-ttu-id="a973a-125">Mail.ReadBasic.All, Mail.Read</span><span class="sxs-lookup"><span data-stu-id="a973a-125">Mail.ReadBasic.All, Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="a973a-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a973a-126">HTTP request</span></span>

<span data-ttu-id="a973a-127">Para obter a mensagem especificada:</span><span class="sxs-lookup"><span data-stu-id="a973a-127">To get the specified message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}
GET /users/{id | userPrincipalName}/messages/{id}
GET /me/mailFolders/{id}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

<span data-ttu-id="a973a-128">Para obter o conteúdo MIME da mensagem especificada:</span><span class="sxs-lookup"><span data-stu-id="a973a-128">To get the MIME content of the specified message:</span></span>
<!-- { "blockType": "ignored" } --> 
```http 
GET /me/messages/{id}/$value 
GET /users/{id | userPrincipalName}/messages/{id}/$value 
GET /me/mailFolders/{id}/messages/{id}/$value 
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/$value 
```

<span data-ttu-id="a973a-129">Para obter uma mensagem e expandir todas as menções na mensagem:</span><span class="sxs-lookup"><span data-stu-id="a973a-129">To get a message and expand all mentions in the message:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/messages/{id}?$expand=mentions
GET /me/mailFolders/{id}/messages/{id}?$expand=mentions
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}?$expand=mentions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a973a-130">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a973a-130">Optional query parameters</span></span>
<span data-ttu-id="a973a-131">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a973a-131">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="a973a-132">Use o parâmetro `$value` para obter o conteúdo MIME de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="a973a-132">Use the `$value` parameter to get the MIME content of a message.</span></span>

<span data-ttu-id="a973a-133">Use o parâmetro de consulta na propriedade de navegação de menções para obter uma mensagem com os detalhes de `$expand` cada menção na mensagem expandida.  [](../resources/mention.md)</span><span class="sxs-lookup"><span data-stu-id="a973a-133">Use the `$expand` query parameter on the **mentions** navigation property to get a message with the details of each [mention](../resources/mention.md) in the message expanded.</span></span>



## <a name="request-headers"></a><span data-ttu-id="a973a-134">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a973a-134">Request headers</span></span>
| <span data-ttu-id="a973a-135">Nome</span><span class="sxs-lookup"><span data-stu-id="a973a-135">Name</span></span>       | <span data-ttu-id="a973a-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="a973a-136">Type</span></span> | <span data-ttu-id="a973a-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="a973a-137">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a973a-138">Autorização</span><span class="sxs-lookup"><span data-stu-id="a973a-138">Authorization</span></span>  | <span data-ttu-id="a973a-139">string</span><span class="sxs-lookup"><span data-stu-id="a973a-139">string</span></span>  | <span data-ttu-id="a973a-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a973a-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a973a-142">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="a973a-142">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="a973a-143">string</span><span class="sxs-lookup"><span data-stu-id="a973a-143">string</span></span> | <span data-ttu-id="a973a-144">O formato das propriedades **body** e **uniqueBody** a serem retornadas.</span><span class="sxs-lookup"><span data-stu-id="a973a-144">The format of the **body** and **uniqueBody** properties to be returned in.</span></span> <span data-ttu-id="a973a-145">Os valores podem ser "text" ou "html".</span><span class="sxs-lookup"><span data-stu-id="a973a-145">Values can be "text" or "html".</span></span> <span data-ttu-id="a973a-146">Um cabeçalho `Preference-Applied` é retornado como confirmação quando este cabeçalho `Prefer` é especificado.</span><span class="sxs-lookup"><span data-stu-id="a973a-146">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="a973a-147">Se o cabeçalho não for especificado, as propriedades **body** e **uniqueBody** serão retornadas no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="a973a-147">If the header is not specified, the **body** and **uniqueBody** properties are returned in HTML format.</span></span> <span data-ttu-id="a973a-148">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a973a-148">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a973a-149">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a973a-149">Request body</span></span>
<span data-ttu-id="a973a-150">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a973a-150">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a973a-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="a973a-151">Response</span></span>

<span data-ttu-id="a973a-152">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [message](../resources/message.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a973a-152">If successful, this method returns a `200 OK` response code and [message](../resources/message.md) object in the response body.</span></span>

<span data-ttu-id="a973a-153">Especificar o parâmetro `$value` retorna o conteúdo da mensagem no formato MIME e não um recurso de **mensagem**.</span><span class="sxs-lookup"><span data-stu-id="a973a-153">Specifying the `$value` parameter returns the message content in MIME format, and not a **message** resource.</span></span>

## <a name="examples"></a><span data-ttu-id="a973a-154">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a973a-154">Examples</span></span>
### <a name="example-1-get-a-specific-message"></a><span data-ttu-id="a973a-155">Exemplo 1: Obter uma mensagem específica</span><span class="sxs-lookup"><span data-stu-id="a973a-155">Example 1: Get a specific message</span></span>
#### <a name="request"></a><span data-ttu-id="a973a-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a973a-156">Request</span></span>
<span data-ttu-id="a973a-157">O primeiro exemplo obtém a mensagem especificada.</span><span class="sxs-lookup"><span data-stu-id="a973a-157">The first example gets the specified message.</span></span> <span data-ttu-id="a973a-158">Ele não especifica nenhum header para indicar o formato desejado do corpo a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="a973a-158">It does not specify any header to indicate the desired format of the body to be returned.</span></span>

# <a name="http"></a>[<span data-ttu-id="a973a-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="a973a-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGI1AAAoZCfHAAA=
```
# <a name="c"></a>[<span data-ttu-id="a973a-160">C#</span><span class="sxs-lookup"><span data-stu-id="a973a-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a973a-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a973a-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a973a-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a973a-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a973a-163">Java</span><span class="sxs-lookup"><span data-stu-id="a973a-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="a973a-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="a973a-164">Response</span></span>
<span data-ttu-id="a973a-165">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a973a-165">Here is an example of the response.</span></span> <span data-ttu-id="a973a-166">As **propriedades body** e **uniqueBody** são retornadas no formato HTML padrão.</span><span class="sxs-lookup"><span data-stu-id="a973a-166">The **body** and **uniqueBody** properties are returned in the default HTML format.</span></span>
<span data-ttu-id="a973a-167">Observação: o objeto de resposta mostrado aqui é truncado para brevidade.</span><span class="sxs-lookup"><span data-stu-id="a973a-167">Note: The response object shown here is truncated for brevity.</span></span> <span data-ttu-id="a973a-168">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a973a-168">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_message",
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


### <a name="example-2-get-all-mentions-in-a-specific-message"></a><span data-ttu-id="a973a-169">Exemplo 2: obter todas as menções em uma mensagem específica</span><span class="sxs-lookup"><span data-stu-id="a973a-169">Example 2: Get all mentions in a specific message</span></span>
#### <a name="request"></a><span data-ttu-id="a973a-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a973a-170">Request</span></span>
<span data-ttu-id="a973a-171">No próximo exemplo, a usuária interna é Dana Swope.</span><span class="sxs-lookup"><span data-stu-id="a973a-171">In the next example, the signed-in user is Dana Swope.</span></span> <span data-ttu-id="a973a-172">O exemplo mostra a obtenção de detalhes de todas as menções na mensagem especificada na caixa de correio da Dana.</span><span class="sxs-lookup"><span data-stu-id="a973a-172">The example shows getting the details of all the mentions in the specified message in Dana's mailbox.</span></span>

# <a name="http"></a>[<span data-ttu-id="a973a-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="a973a-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AQMkADJmMTUAAAgVZAAAA"],
  "name": "get_mentions_in_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AQMkADJmMTUAAAgVZAAAA/?$expand=mentions
```
# <a name="c"></a>[<span data-ttu-id="a973a-174">C#</span><span class="sxs-lookup"><span data-stu-id="a973a-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mentions-in-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a973a-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a973a-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mentions-in-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a973a-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a973a-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mentions-in-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a973a-177">Java</span><span class="sxs-lookup"><span data-stu-id="a973a-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-mentions-in-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="a973a-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="a973a-178">Response</span></span>
<span data-ttu-id="a973a-179">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a973a-179">Here is an example of the response.</span></span> <span data-ttu-id="a973a-180">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a973a-180">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_mentions_in_message",
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

### <a name="example-3-get-message-body-in-text-format"></a><span data-ttu-id="a973a-181">Exemplo 3: Obter o corpo da mensagem em formato de texto</span><span class="sxs-lookup"><span data-stu-id="a973a-181">Example 3: Get message body in text format</span></span>
#### <a name="request"></a><span data-ttu-id="a973a-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a973a-182">Request</span></span>

<span data-ttu-id="a973a-183">O terceiro exemplo mostra como usar um `Prefer: outlook.body-content-type="text"` cabeçalho para obter o **corpo** e o **uniqueBody** da mensagem especificada no formato do texto.</span><span class="sxs-lookup"><span data-stu-id="a973a-183">The third example shows how to use a `Prefer: outlook.body-content-type="text"` header to get the **body** and **uniqueBody** of the specified message in text format.</span></span>


# <a name="http"></a>[<span data-ttu-id="a973a-184">HTTP</span><span class="sxs-lookup"><span data-stu-id="a973a-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGI1AAAoZCfHAAA="],
  "name": "get_message_in_text"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGI1AAAoZCfHAAA=/?$select=subject,body,bodyPreview,uniqueBody
Prefer: outlook.body-content-type="text"
```
# <a name="c"></a>[<span data-ttu-id="a973a-185">C#</span><span class="sxs-lookup"><span data-stu-id="a973a-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-in-text-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a973a-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a973a-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-in-text-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a973a-187">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a973a-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-in-text-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a973a-188">Java</span><span class="sxs-lookup"><span data-stu-id="a973a-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-in-text-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a973a-189">Resposta</span><span class="sxs-lookup"><span data-stu-id="a973a-189">Response</span></span>

<span data-ttu-id="a973a-190">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a973a-190">Here is an example of the response.</span></span> <span data-ttu-id="a973a-191">Observação: a resposta inclui um `Preference-Applied: outlook.body-content-type` cabeçalho para reconhecer o `Prefer: outlook.body-content-type` cabeçalho da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a973a-191">Note: The response includes a `Preference-Applied: outlook.body-content-type` header to acknowledge the `Prefer: outlook.body-content-type` request header.</span></span>
<!-- {
  "blockType": "response",
  "name": "get_message_in_text",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Preference-Applied: outlook.body-content-type="text"

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
### <a name="example-4-get-internet-message-headers"></a><span data-ttu-id="a973a-192">Exemplo 4: Obter os headers de mensagens da Internet</span><span class="sxs-lookup"><span data-stu-id="a973a-192">Example 4: Get Internet message headers</span></span>
#### <a name="request"></a><span data-ttu-id="a973a-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a973a-193">Request</span></span>

<span data-ttu-id="a973a-194">O quarto exemplo mostra como obter os headers de mensagens da Internet de uma mensagem específica.</span><span class="sxs-lookup"><span data-stu-id="a973a-194">The fourth example shows how to get the Internet message headers of a specific message.</span></span>  


# <a name="http"></a>[<span data-ttu-id="a973a-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="a973a-195">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEz"],
  "name": "get_message_internet_headers"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/AAMkAGVmMDEz/?$select=internetMessageHeaders
```
# <a name="c"></a>[<span data-ttu-id="a973a-196">C#</span><span class="sxs-lookup"><span data-stu-id="a973a-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-internet-headers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a973a-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a973a-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-internet-headers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a973a-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a973a-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-internet-headers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a973a-199">Java</span><span class="sxs-lookup"><span data-stu-id="a973a-199">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-internet-headers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a973a-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="a973a-200">Response</span></span>

<span data-ttu-id="a973a-201">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a973a-201">Here is an example of the response.</span></span> <span data-ttu-id="a973a-202">Observação: o número de headers de mensagens da Internet no objeto de resposta foi reduzido por brevidade.</span><span class="sxs-lookup"><span data-stu-id="a973a-202">Note: The number of Internet message headers in the response object has been reduced for brevity.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_message_internet_headers",
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


### <a name="example-5-get-mime-content"></a><span data-ttu-id="a973a-203">Exemplo 5: Obter conteúdo MIME</span><span class="sxs-lookup"><span data-stu-id="a973a-203">Example 5: Get MIME content</span></span>
#### <a name="request"></a><span data-ttu-id="a973a-204">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a973a-204">Request</span></span>
<span data-ttu-id="a973a-205">O quinto exemplo obtém o conteúdo MIME de uma mensagem na caixa de correio do usuário de entrada.</span><span class="sxs-lookup"><span data-stu-id="a973a-205">The fifth example gets the MIME content of a message in the signed-in user's mailbox.</span></span>


# <a name="http"></a>[<span data-ttu-id="a973a-206">HTTP</span><span class="sxs-lookup"><span data-stu-id="a973a-206">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_message_in_mime",
  "sampleKeys": ["4aade2547798441eab5188a7a2436bc1"]
} -->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/messages/4aade2547798441eab5188a7a2436bc1/$value
```
# <a name="c"></a>[<span data-ttu-id="a973a-207">C#</span><span class="sxs-lookup"><span data-stu-id="a973a-207">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-message-in-mime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a973a-208">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a973a-208">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-message-in-mime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a973a-209">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a973a-209">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-message-in-mime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a973a-210">Java</span><span class="sxs-lookup"><span data-stu-id="a973a-210">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-message-in-mime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a973a-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="a973a-211">Response</span></span>
<span data-ttu-id="a973a-212">Esta é a resposta.</span><span class="sxs-lookup"><span data-stu-id="a973a-212">The following is the response.</span></span> <span data-ttu-id="a973a-213">O conteúdo MIME começa com o `MIME-Version` cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="a973a-213">The MIME content begins with the `MIME-Version` header.</span></span> 
<!-- {
  "blockType": "response",
  "name": "get_message_in_mime",
  "truncated": true,
  "@odata.type": "string"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

Received: from contoso.com (10.194.241.197) by 
contoso.com (10.194.241.197) with Microsoft 
SMTP Server (version=TLS1_2, 
cipher=TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384_P256) id 15.1.1374.0 via Mailbox 
Transport; Mon, 4 Sep 2017 03:00:08 -0700 
Received: from contoso.com (10.194.241.197) by 
contoso.com (10.194.241.197) with Microsoft 
SMTP Server (version=TLS1_2, 
cipher=TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384_P256) id 15.1.1374.0; Mon, 4 Sep 
2017 03:00:07 -0700 
Received: from contoso.com 
(fe80::5bf:5059:4ca0:5017) by contoso.com 
(fe80::5bf:5059:4ca0:5017%12) with mapi id 15.01.1374.000; Mon, 4 Sep 2017 
03:00:01 -0700 
From: Administrator <admin@contoso.com> 
To: Administrator <admin@contoso.com> 
Subject: This email has attachment. 
Thread-Topic: This email has attachment. 
Thread-Index: AQHTJWSHSywMzSz8o0OJud48nG50GQ== 
Date: Mon, 4 Sep 2017 10:00:00 +0000 
Message-ID: 
                <4aade2547798441eab5188a7a2436bc1@contoso.com> 
Accept-Language: en-US 
Content-Language: en-US 
X-MS-Exchange-Organization-AuthAs: Internal 
X-MS-Exchange-Organization-AuthMechanism: 04 
X-MS-Exchange-Organization-AuthSource: 
                contoso.com 
X-MS-Has-Attach: yes 
X-MS-Exchange-Organization-Network-Message-Id: 
                0ffdb402-ec03-42c8-5d32-08d4f37bb517 
X-MS-Exchange-Organization-SCL: -1 
X-MS-TNEF-Correlator: 
X-MS-Exchange-Organization-RecordReviewCfmType: 0 

MIME-Version: 1.0 
Content-Type: multipart/mixed; 
                boundary="_004_4aade2547798441eab5188a7a2436bc1contoso_" 
 
--_004_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: multipart/alternative; 
                boundary="_000_4aade2547798441eab5188a7a2436bc1contoso_" 
 
--_000_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: text/plain; charset="iso-8859-1" 
Content-Transfer-Encoding: quoted-printable 
 
The attachment is an email. 
 
--_000_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: text/html; charset="iso-8859-1" 
Content-Transfer-Encoding: quoted-printable 
 
<html> 
<head> 
<meta http-equiv=3D"Content-Type" content=3D"text/html; charset=3Diso-8859-= 
1"> 
<style type=3D"text/css" style=3D"display:none;"><!-- P {margin-top:0;margi= 
n-bottom:0;} --></style> 
</head> 
<body dir=3D"ltr"> 
<div id=3D"divtagdefaultwrapper" style=3D"font-size:12pt;color:#000000;font= 
-family:Calibri,Helvetica,sans-serif;" dir=3D"ltr"> 
<p>The attachment is an email.</p> 
</div> 
</body> 
</html> 
 
--_000_4aade2547798441eab5188a7a2436bc1contoso_-- 
 
--_004_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: application/octet-stream; name="Attachment email.eml" 
Content-Description: Attachment email.eml 
Content-Disposition: attachment; filename="Attachment email.eml"; size=408; 
                creation-date="Mon, 04 Sep 2017 09:59:43 GMT"; 
                modification-date="Mon, 04 Sep 2017 09:59:43 GMT" 
Content-Transfer-Encoding: base64 
 
RnJvbToJQWRtaW5pc3RyYXRvciA8YWRtaW5AdGVuYW50LUVYSEItMTQ3MS5jb20+DQpTZW50OglN 
b25kYXksIFNlcHRlbWJlciA0LCAyMDE3IDM6MjYgUE0NClRvOglTcml2YXJkaGFuIEhlYmJhcg0K 
U3ViamVjdDoJQXR0YWNobWVudCBlbWFpbA0KDQpJIHdpbGwgYXR0YWNoIHRoaXMgZW1haWwgdG8g 
YW5vdGhlciBtYWlsLg0K 
 
--_004_4aade2547798441eab5188a7a2436bc1contoso_-- 
```


## <a name="see-also"></a><span data-ttu-id="a973a-214">Confira também</span><span class="sxs-lookup"><span data-stu-id="a973a-214">See also</span></span>

- [<span data-ttu-id="a973a-215">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="a973a-215">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="a973a-216">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="a973a-216">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="a973a-217">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="a973a-217">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

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
    "Error: get_message_internet_headers/internetMessageHeaders/member/value:\r\n       Expected type String but actual was Binary. Property: value, actual value: 'binary'"
  ]
}
-->


