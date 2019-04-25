---
title: 'usuário: getDicas de dicas'
description: Obter as Dicas de E-mail de um ou mais destinatários como disponíveis para o usuário conectado.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4c931d6e7f3b7762534d773b647f7db68461a230
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567862"
---
# <a name="user-getmailtips"></a><span data-ttu-id="c6e62-103">usuário: getDicas de dicas</span><span class="sxs-lookup"><span data-stu-id="c6e62-103">user: getMailTips</span></span>

<span data-ttu-id="c6e62-104">Obtenha as dicas de informações de um ou mais destinatários como disponíveis para o [usuário](../resources/user.md)conectado.</span><span class="sxs-lookup"><span data-stu-id="c6e62-104">Get the MailTips of one or more recipients as available to the signed-in [user](../resources/user.md).</span></span>

<span data-ttu-id="c6e62-105">Observe que fazendo uma `POST` chamada para a `getMailTips` ação, você pode solicitar tipos específicos de dicas de anotações a serem retornados para mais de um destinatário ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="c6e62-105">Note that by making a `POST` call to the `getMailTips` action, you can request specific types of MailTips to be returned for more than one recipient at one time.</span></span> <span data-ttu-id="c6e62-106">As dicas de entrada solicitadas são retornadas em uma coleção de [dicas de dicas](../resources/mailtips.md) .</span><span class="sxs-lookup"><span data-stu-id="c6e62-106">The requested MailTips are returned in a [mailTips](../resources/mailtips.md) collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6e62-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c6e62-107">Permissions</span></span>
<span data-ttu-id="c6e62-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6e62-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6e62-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6e62-110">Permission type</span></span>      | <span data-ttu-id="c6e62-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c6e62-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6e62-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6e62-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c6e62-113">Mail. Read, mail. Read. Shared</span><span class="sxs-lookup"><span data-stu-id="c6e62-113">Mail.Read, Mail.Read.Shared</span></span>    |
|<span data-ttu-id="c6e62-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6e62-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6e62-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c6e62-115">Mail.Read</span></span>    |
|<span data-ttu-id="c6e62-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6e62-116">Application</span></span> | <span data-ttu-id="c6e62-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="c6e62-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6e62-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6e62-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMailTips
POST /users/{id|userPrincipalName}/getMailTips
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c6e62-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c6e62-119">Optional query parameters</span></span>
<span data-ttu-id="c6e62-120">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c6e62-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c6e62-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6e62-121">Request headers</span></span>
| <span data-ttu-id="c6e62-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c6e62-122">Header</span></span>       | <span data-ttu-id="c6e62-123">Valor</span><span class="sxs-lookup"><span data-stu-id="c6e62-123">Value</span></span>|
|:-----------  |:------|
| <span data-ttu-id="c6e62-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6e62-124">Authorization</span></span> | <span data-ttu-id="c6e62-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6e62-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c6e62-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c6e62-127">Content-Type</span></span>  | <span data-ttu-id="c6e62-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c6e62-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c6e62-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6e62-129">Request body</span></span>
<span data-ttu-id="c6e62-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c6e62-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c6e62-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6e62-131">Property</span></span>     | <span data-ttu-id="c6e62-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6e62-132">Type</span></span>   |<span data-ttu-id="c6e62-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6e62-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6e62-134">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="c6e62-134">EmailAddresses</span></span>|<span data-ttu-id="c6e62-135">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="c6e62-135">String collection</span></span>|<span data-ttu-id="c6e62-136">Uma coleção de endereços SMTP de destinatários para receber as Dicas de Email.</span><span class="sxs-lookup"><span data-stu-id="c6e62-136">A collection of SMTP addresses of recipients to get MailTips for.</span></span>|
|<span data-ttu-id="c6e62-137">MailTipsOptions</span><span class="sxs-lookup"><span data-stu-id="c6e62-137">MailTipsOptions</span></span>|<span data-ttu-id="c6e62-138">String</span><span class="sxs-lookup"><span data-stu-id="c6e62-138">String</span></span>|<span data-ttu-id="c6e62-139">Uma enumeração de sinalizadores que representa as dicas de as as solicitadas.</span><span class="sxs-lookup"><span data-stu-id="c6e62-139">A enumeration of flags that represents the requested mailtips.</span></span> <span data-ttu-id="c6e62-140">Os valores possíveis são `automaticReplies`: `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, e `totalMemberCount`.</span><span class="sxs-lookup"><span data-stu-id="c6e62-140">Possible values are: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, and `totalMemberCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="c6e62-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6e62-141">Response</span></span>

<span data-ttu-id="c6e62-142">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos de [dicas](../resources/mailtips.md) de mensagem no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6e62-142">If successful, this method returns a `200 OK` response code and a collection of [mailTips](../resources/mailtips.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c6e62-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c6e62-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6e62-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6e62-144">Request</span></span>
<span data-ttu-id="c6e62-145">O exemplo a seguir obtém dicas de correio para os destinatários especificados, para qualquer configuração de resposta automática e o status completo da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c6e62-145">The following example gets MailTips for the specified recipients, for any automatic reply settings and the mailbox full status.</span></span>

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

##### <a name="response"></a><span data-ttu-id="c6e62-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6e62-146">Response</span></span>
<span data-ttu-id="c6e62-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c6e62-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
