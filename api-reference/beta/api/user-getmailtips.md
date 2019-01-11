---
title: 'usuário: getMailTips'
description: Obter as Dicas de E-mail de um ou mais destinatários como disponíveis para o usuário conectado.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 2577b37f6cbfa3bd6dc5eff712c07562ecdadbf2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855962"
---
# <a name="user-getmailtips"></a><span data-ttu-id="8fbaa-103">usuário: getMailTips</span><span class="sxs-lookup"><span data-stu-id="8fbaa-103">user: getMailTips</span></span>

> <span data-ttu-id="8fbaa-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8fbaa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8fbaa-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8fbaa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8fbaa-106">Obtenha dicas de email de um ou mais destinatários conforme disponível ao entrou no [usuário](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="8fbaa-106">Get the MailTips of one or more recipients as available to the signed-in [user](../resources/user.md).</span></span>

<span data-ttu-id="8fbaa-107">Observe que, tornando uma `POST` chamada para o `getMailTips` ação, você poderá solicitar tipos específicos de dicas de email a ser retornado por mais de um destinatário de uma só vez.</span><span class="sxs-lookup"><span data-stu-id="8fbaa-107">Note that by making a `POST` call to the `getMailTips` action, you can request specific types of MailTips to be returned for more than one recipient at one time.</span></span> <span data-ttu-id="8fbaa-108">As dicas de email solicitadas são retornadas em uma coleção de [dicas de email](../resources/mailtips.md) .</span><span class="sxs-lookup"><span data-stu-id="8fbaa-108">The requested MailTips are returned in a [mailTips](../resources/mailtips.md) collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="8fbaa-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="8fbaa-109">Permissions</span></span>
<span data-ttu-id="8fbaa-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8fbaa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fbaa-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8fbaa-112">Permission type</span></span>      | <span data-ttu-id="8fbaa-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8fbaa-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8fbaa-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8fbaa-114">Delegated (work or school account)</span></span> | <span data-ttu-id="8fbaa-115">Mail.Read, Mail.Read.Shared</span><span class="sxs-lookup"><span data-stu-id="8fbaa-115">Mail.Read, Mail.Read.Shared</span></span>    |
|<span data-ttu-id="8fbaa-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8fbaa-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fbaa-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8fbaa-117">Mail.Read</span></span>    |
|<span data-ttu-id="8fbaa-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8fbaa-118">Application</span></span> | <span data-ttu-id="8fbaa-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="8fbaa-119">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="8fbaa-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8fbaa-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMailTips
POST /users/{id|userPrincipalName}/getMailTips
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8fbaa-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8fbaa-121">Optional query parameters</span></span>
<span data-ttu-id="8fbaa-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8fbaa-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8fbaa-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8fbaa-123">Request headers</span></span>
| <span data-ttu-id="8fbaa-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8fbaa-124">Header</span></span>       | <span data-ttu-id="8fbaa-125">Valor</span><span class="sxs-lookup"><span data-stu-id="8fbaa-125">Value</span></span>|
|:-----------  |:------|
| <span data-ttu-id="8fbaa-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="8fbaa-126">Authorization</span></span> | <span data-ttu-id="8fbaa-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8fbaa-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8fbaa-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8fbaa-129">Content-Type</span></span>  | <span data-ttu-id="8fbaa-130">application/json</span><span class="sxs-lookup"><span data-stu-id="8fbaa-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8fbaa-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8fbaa-131">Request body</span></span>
<span data-ttu-id="8fbaa-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8fbaa-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8fbaa-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8fbaa-133">Property</span></span>     | <span data-ttu-id="8fbaa-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="8fbaa-134">Type</span></span>   |<span data-ttu-id="8fbaa-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="8fbaa-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8fbaa-136">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="8fbaa-136">EmailAddresses</span></span>|<span data-ttu-id="8fbaa-137">String collection</span><span class="sxs-lookup"><span data-stu-id="8fbaa-137">String collection</span></span>|<span data-ttu-id="8fbaa-138">Uma coleção de endereços SMTP de destinatários para receber as Dicas de Email.</span><span class="sxs-lookup"><span data-stu-id="8fbaa-138">A collection of SMTP addresses of recipients to get MailTips for.</span></span>|
|<span data-ttu-id="8fbaa-139">MailTipsOptions</span><span class="sxs-lookup"><span data-stu-id="8fbaa-139">MailTipsOptions</span></span>|<span data-ttu-id="8fbaa-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8fbaa-140">String</span></span>|<span data-ttu-id="8fbaa-141">Enumeração dos sinalizadores que representa as dicas de email solicitadas.</span><span class="sxs-lookup"><span data-stu-id="8fbaa-141">A enumeration of flags that represents the requested mailtips.</span></span> <span data-ttu-id="8fbaa-142">Os valores possíveis são: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, e `totalMemberCount`.</span><span class="sxs-lookup"><span data-stu-id="8fbaa-142">Possible values are: `automaticReplies`, `customMailTip`, `deliveryRestriction`, `externalMemberCount`, `mailboxFullStatus`, `maxMessageSize`, `moderationStatus`, `recipientScope`, `recipientSuggestions`, and `totalMemberCount`.</span></span>|

## <a name="response"></a><span data-ttu-id="8fbaa-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fbaa-143">Response</span></span>

<span data-ttu-id="8fbaa-144">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos de [dicas de email](../resources/mailtips.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8fbaa-144">If successful, this method returns a `200 OK` response code and a collection of [mailTips](../resources/mailtips.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8fbaa-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8fbaa-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8fbaa-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8fbaa-146">Request</span></span>
<span data-ttu-id="8fbaa-147">O exemplo a seguir obtém as dicas de email para os destinatários especificados, para quaisquer configurações de resposta automática e o status completo de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="8fbaa-147">The following example gets MailTips for the specified recipients, for any automatic reply settings and the mailbox full status.</span></span>

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

##### <a name="response"></a><span data-ttu-id="8fbaa-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="8fbaa-148">Response</span></span>
<span data-ttu-id="8fbaa-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8fbaa-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: getMailTips",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
