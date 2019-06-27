---
title: 'usuário: getdicas de dicas'
description: Obter as Dicas de E-mail de um ou mais destinatários como disponíveis para o usuário conectado.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1ba2e8889be298c9c601d7db8cdecff62498ff4c
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270319"
---
# <a name="user-getmailtips"></a><span data-ttu-id="29f7e-103">usuário: getdicas de dicas</span><span class="sxs-lookup"><span data-stu-id="29f7e-103">user: getMailTips</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29f7e-104">Obtenha as dicas de informações de um ou mais destinatários como disponíveis para o [usuário](../resources/user.md)conectado.</span><span class="sxs-lookup"><span data-stu-id="29f7e-104">Get the MailTips of one or more recipients as available to the signed-in [user](../resources/user.md).</span></span>

<span data-ttu-id="29f7e-105">Observe que fazendo uma `POST` chamada para a `getMailTips` ação, você pode solicitar tipos específicos de dicas de anotações a serem retornados para mais de um destinatário ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="29f7e-105">Note that by making a `POST` call to the `getMailTips` action, you can request specific types of MailTips to be returned for more than one recipient at one time.</span></span> <span data-ttu-id="29f7e-106">As dicas de entrada solicitadas são retornadas em uma coleção de [dicas de dicas](../resources/mailtips.md) .</span><span class="sxs-lookup"><span data-stu-id="29f7e-106">The requested MailTips are returned in a [mailTips](../resources/mailtips.md) collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="29f7e-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="29f7e-107">Permissions</span></span>
<span data-ttu-id="29f7e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29f7e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29f7e-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29f7e-110">Permission type</span></span>      | <span data-ttu-id="29f7e-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="29f7e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29f7e-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29f7e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="29f7e-113">Mail. Read, mail. Read. Shared</span><span class="sxs-lookup"><span data-stu-id="29f7e-113">Mail.Read, Mail.Read.Shared</span></span>    |
|<span data-ttu-id="29f7e-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29f7e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29f7e-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="29f7e-115">Mail.Read</span></span>    |
|<span data-ttu-id="29f7e-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29f7e-116">Application</span></span> | <span data-ttu-id="29f7e-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="29f7e-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="29f7e-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29f7e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMailTips
POST /users/{id|userPrincipalName}/getMailTips
```
## <a name="optional-query-parameters"></a><span data-ttu-id="29f7e-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="29f7e-119">Optional query parameters</span></span>
<span data-ttu-id="29f7e-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="29f7e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="29f7e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29f7e-121">Request headers</span></span>
| <span data-ttu-id="29f7e-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="29f7e-122">Header</span></span>       | <span data-ttu-id="29f7e-123">Valor</span><span class="sxs-lookup"><span data-stu-id="29f7e-123">Value</span></span>|
|:-----------  |:------|
| <span data-ttu-id="29f7e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="29f7e-124">Authorization</span></span> | <span data-ttu-id="29f7e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29f7e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="29f7e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="29f7e-127">Content-Type</span></span>  | <span data-ttu-id="29f7e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="29f7e-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="29f7e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29f7e-129">Request body</span></span>
<span data-ttu-id="29f7e-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29f7e-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="29f7e-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29f7e-131">Property</span></span>     | <span data-ttu-id="29f7e-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="29f7e-132">Type</span></span>   |<span data-ttu-id="29f7e-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="29f7e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29f7e-134">EndereçosEmail</span><span class="sxs-lookup"><span data-stu-id="29f7e-134">EmailAddresses</span></span>|<span data-ttu-id="29f7e-135">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="29f7e-135">String collection</span></span>|<span data-ttu-id="29f7e-136">Uma coleção de endereços SMTP de destinatários para receber as Dicas de Email.</span><span class="sxs-lookup"><span data-stu-id="29f7e-136">A collection of SMTP addresses of recipients to get MailTips for.</span></span>|
|<span data-ttu-id="29f7e-137">MailTipsOptions</span><span class="sxs-lookup"><span data-stu-id="29f7e-137">MailTipsOptions</span></span>|<span data-ttu-id="29f7e-138">String</span><span class="sxs-lookup"><span data-stu-id="29f7e-138">String</span></span>|<span data-ttu-id="29f7e-139">Uma enumeração de sinalizadores que representa as dicas de as as solicitadas.</span><span class="sxs-lookup"><span data-stu-id="29f7e-139">A enumeration of flags that represents the requested mailtips.</span></span> <span data-ttu-id="29f7e-140">Os valores possíveis são `automaticReplies`: `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, e `totalMemberCount`.</span><span class="sxs-lookup"><span data-stu-id="29f7e-140">Possible values are: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, and `totalMemberCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="29f7e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="29f7e-141">Response</span></span>

<span data-ttu-id="29f7e-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos de [dicas](../resources/mailtips.md) de mensagem no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29f7e-142">If successful, this method returns a `200 OK` response code and a collection of [mailTips](../resources/mailtips.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="29f7e-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29f7e-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="29f7e-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29f7e-144">Request</span></span>
<span data-ttu-id="29f7e-145">O exemplo a seguir obtém dicas de correio para os destinatários especificados, para qualquer configuração de resposta automática e o status completo da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="29f7e-145">The following example gets MailTips for the specified recipients, for any automatic reply settings and the mailbox full status.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_getmailtips"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMailTips
Content-Type: application/json

{
    "EmailAddresses": [
        "danas@contoso.onmicrosoft.com", 
        "fannyd@contoso.onmicrosoft.com"
    ],
    "MailTipsOptions": "automaticReplies, mailboxFullStatus"
}
```

##### <a name="response"></a><span data-ttu-id="29f7e-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="29f7e-146">Response</span></span>
<span data-ttu-id="29f7e-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29f7e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.mailTips)",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="29f7e-150">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="29f7e-150">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="29f7e-151">C#</span><span class="sxs-lookup"><span data-stu-id="29f7e-151">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_getmailtips-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="29f7e-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="29f7e-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_getmailtips-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="29f7e-153">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="29f7e-153">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_getmailtips-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: getMailTips",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-getmailtips.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-getmailtips.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-getmailtips.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
