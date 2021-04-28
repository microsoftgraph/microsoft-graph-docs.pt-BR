---
title: 'user: getMailTips'
description: Obter as Dicas de E-mail de um ou mais destinatários como disponíveis para o usuário conectado.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fd46d262cf7d190daa4c5f21e1c45ec1472b799f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055684"
---
# <a name="user-getmailtips"></a><span data-ttu-id="dc510-103">user: getMailTips</span><span class="sxs-lookup"><span data-stu-id="dc510-103">user: getMailTips</span></span>

<span data-ttu-id="dc510-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc510-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dc510-105">Obter as Dicas de Email de um ou mais destinatários, conforme disponível para o usuário [de logom.](../resources/user.md)</span><span class="sxs-lookup"><span data-stu-id="dc510-105">Get the MailTips of one or more recipients as available to the signed-in [user](../resources/user.md).</span></span>

<span data-ttu-id="dc510-106">Observe que, ao fazer uma chamada para a ação, você pode solicitar que tipos específicos de Dicas de Email sejam retornados por mais de `POST` um destinatário de cada `getMailTips` vez.</span><span class="sxs-lookup"><span data-stu-id="dc510-106">Note that by making a `POST` call to the `getMailTips` action, you can request specific types of MailTips to be returned for more than one recipient at one time.</span></span> <span data-ttu-id="dc510-107">As Dicas de Email solicitadas são retornadas em uma coleção [mailTips.](../resources/mailtips.md)</span><span class="sxs-lookup"><span data-stu-id="dc510-107">The requested MailTips are returned in a [mailTips](../resources/mailtips.md) collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc510-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="dc510-108">Permissions</span></span>
<span data-ttu-id="dc510-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc510-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc510-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc510-111">Permission type</span></span>      | <span data-ttu-id="dc510-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dc510-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc510-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc510-113">Delegated (work or school account)</span></span> | <span data-ttu-id="dc510-114">Mail.Read, Mail.Read.Shared</span><span class="sxs-lookup"><span data-stu-id="dc510-114">Mail.Read, Mail.Read.Shared</span></span>    |
|<span data-ttu-id="dc510-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc510-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc510-116">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="dc510-116">Mail.Read</span></span>    |
|<span data-ttu-id="dc510-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc510-117">Application</span></span> | <span data-ttu-id="dc510-118">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="dc510-118">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc510-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc510-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMailTips
POST /users/{id|userPrincipalName}/getMailTips
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dc510-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dc510-120">Optional query parameters</span></span>
<span data-ttu-id="dc510-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dc510-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="dc510-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc510-122">Request headers</span></span>
| <span data-ttu-id="dc510-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dc510-123">Header</span></span>       | <span data-ttu-id="dc510-124">Valor</span><span class="sxs-lookup"><span data-stu-id="dc510-124">Value</span></span>|
|:-----------  |:------|
| <span data-ttu-id="dc510-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc510-125">Authorization</span></span> | <span data-ttu-id="dc510-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc510-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dc510-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dc510-128">Content-Type</span></span>  | <span data-ttu-id="dc510-129">application/json</span><span class="sxs-lookup"><span data-stu-id="dc510-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dc510-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc510-130">Request body</span></span>
<span data-ttu-id="dc510-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc510-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="dc510-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc510-132">Property</span></span>     | <span data-ttu-id="dc510-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc510-133">Type</span></span>   |<span data-ttu-id="dc510-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc510-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc510-135">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="dc510-135">EmailAddresses</span></span>|<span data-ttu-id="dc510-136">Coleção String</span><span class="sxs-lookup"><span data-stu-id="dc510-136">String collection</span></span>|<span data-ttu-id="dc510-137">Uma coleção de endereços SMTP de destinatários para receber as Dicas de Email.</span><span class="sxs-lookup"><span data-stu-id="dc510-137">A collection of SMTP addresses of recipients to get MailTips for.</span></span>|
|<span data-ttu-id="dc510-138">MailTipsOptions</span><span class="sxs-lookup"><span data-stu-id="dc510-138">MailTipsOptions</span></span>|<span data-ttu-id="dc510-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc510-139">String</span></span>|<span data-ttu-id="dc510-140">Uma enumeração de sinalizadores que representa as dicas de email solicitadas.</span><span class="sxs-lookup"><span data-stu-id="dc510-140">A enumeration of flags that represents the requested mailtips.</span></span> <span data-ttu-id="dc510-141">Os valores possíveis são: `automaticReplies` , , , , , , , , , `customMailTip` e `deliveryRestriction` `externalMemberCount` `mailboxFullStatus` `maxMessageSize` `moderationStatus` `recipientScope` `recipientSuggestions` `totalMemberCount` .</span><span class="sxs-lookup"><span data-stu-id="dc510-141">Possible values are: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, and `totalMemberCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="dc510-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc510-142">Response</span></span>

<span data-ttu-id="dc510-143">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos mailTips](../resources/mailtips.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc510-143">If successful, this method returns a `200 OK` response code and a collection of [mailTips](../resources/mailtips.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dc510-144">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc510-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dc510-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc510-145">Request</span></span>
<span data-ttu-id="dc510-146">O exemplo a seguir obtém Dicas de Email para os destinatários especificados, para qualquer configuração de resposta automática e o status completo da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="dc510-146">The following example gets MailTips for the specified recipients, for any automatic reply settings and the mailbox full status.</span></span>


# <a name="http"></a>[<span data-ttu-id="dc510-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc510-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_getmailtips"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMailTips
Content-Type: application/json

{
    "EmailAddresses": [
        "danas@contoso.onmicrosoft.com", 
        "fannyd@contoso.onmicrosoft.com"
    ],
    "MailTipsOptions": "automaticReplies, mailboxFullStatus"
}
```
# <a name="c"></a>[<span data-ttu-id="dc510-148">C#</span><span class="sxs-lookup"><span data-stu-id="dc510-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-getmailtips-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dc510-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc510-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-getmailtips-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dc510-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc510-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-getmailtips-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dc510-151">Java</span><span class="sxs-lookup"><span data-stu-id="dc510-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-getmailtips-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dc510-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc510-152">Response</span></span>
<span data-ttu-id="dc510-153">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc510-153">Here is an example of the response.</span></span> <span data-ttu-id="dc510-154">Observação: o objeto de resposta exibido aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dc510-154">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailTips",
  isCollection: true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.mailTips)",
    "value":[
        {
            "emailAddress":{
                "name":"",
                "address":"danas@contoso.onmicrosoft.com"
            },
            "automaticReplies":{
                "message":"<style type=\"text/css\" style=\"\">\r\n<!--\r\np\r\n\t{margin-top:0;\r\n\tmargin-bottom:0}\r\n-->\r\n</style>\r\n<div dir=\"ltr\">\r\n<div id=\"x_divtagdefaultwrapper\" style=\"font-size:12pt; color:#000000; background-color:#FFFFFF; font-family:Calibri,Arial,Helvetica,sans-serif\">\r\n<p>Hi, I am on vacation right now. I'll get back to you after I return.<br>\r\n</p>\r\n</div>\r\n</div>",
                "messageLanguage":{
                    "locale":"en-US",
                    "displayName":"English (United States)"
                },
                "scheduledStartTime": {
                    "dateTime": "2018-08-07T02:00:00.0000000",
                    "timeZone": "UTC"
                },
                "scheduledEndTime": {
                    "dateTime": "2018-08-09T02:00:00.0000000",
                    "timeZone": "UTC"
                }
            },
            "mailboxFull":false
        },
        {
            "emailAddress":{
                "name":"",
                "address":"fannyd@contoso.onmicrosoft.com"
            },
            "automaticReplies":{
                "message":""
            },
            "mailboxFull":false
        }
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: getMailTips",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
