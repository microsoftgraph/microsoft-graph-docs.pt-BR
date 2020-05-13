---
title: Obter regra
description: Obtenha as propriedades e as relações de um objeto messageRule.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 932337a15ac558d8f92c3b0f76a2c40b7ad74984
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "43448439"
---
# <a name="get-rule"></a><span data-ttu-id="c84fa-103">Obter regra</span><span class="sxs-lookup"><span data-stu-id="c84fa-103">Get rule</span></span>

<span data-ttu-id="c84fa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c84fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c84fa-105">Obtenha as propriedades e as relações de um objeto [messageRule](../resources/messagerule.md).</span><span class="sxs-lookup"><span data-stu-id="c84fa-105">Get the properties and relationships of a [messageRule](../resources/messagerule.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="c84fa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c84fa-106">Permissions</span></span>
<span data-ttu-id="c84fa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c84fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c84fa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c84fa-109">Permission type</span></span>      | <span data-ttu-id="c84fa-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c84fa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c84fa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c84fa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c84fa-112">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="c84fa-112">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="c84fa-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c84fa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c84fa-114">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="c84fa-114">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="c84fa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c84fa-115">Application</span></span> | <span data-ttu-id="c84fa-116">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="c84fa-116">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="c84fa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c84fa-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messagerules/{id}
GET /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c84fa-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c84fa-118">Optional query parameters</span></span>
<span data-ttu-id="c84fa-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c84fa-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c84fa-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c84fa-120">Request headers</span></span>
| <span data-ttu-id="c84fa-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c84fa-121">Name</span></span>      |<span data-ttu-id="c84fa-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c84fa-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c84fa-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c84fa-123">Authorization</span></span>  | <span data-ttu-id="c84fa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c84fa-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="c84fa-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c84fa-126">Request body</span></span>
<span data-ttu-id="c84fa-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c84fa-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c84fa-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c84fa-128">Response</span></span>
<span data-ttu-id="c84fa-129">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [messageRule](../resources/messagerule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c84fa-129">If successful, this method returns a `200 OK` response code and [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c84fa-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c84fa-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c84fa-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c84fa-131">Request</span></span>
<span data-ttu-id="c84fa-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c84fa-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c84fa-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c84fa-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messagerule"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')
```
# <a name="c"></a>[<span data-ttu-id="c84fa-134">C#</span><span class="sxs-lookup"><span data-stu-id="c84fa-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c84fa-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c84fa-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c84fa-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c84fa-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c84fa-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c84fa-137">Response</span></span>
<span data-ttu-id="c84fa-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c84fa-138">Here is an example of the response.</span></span> <span data-ttu-id="c84fa-139">Por padrão, as propriedades de data e hora na resposta estão em UTC.</span><span class="sxs-lookup"><span data-stu-id="c84fa-139">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="c84fa-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c84fa-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Me/mailFolders('inbox')/messageRules/$entity",
  "id":"AQAAAJ5dZqA=",
  "displayName":"From partner",
  "sequence":2,
  "isEnabled":true,
  "hasError":false,
  "isReadOnly":false,
  "conditions":{
    "senderContains":[
      "ADELE"
    ]
  },
  "actions":{
    "stopProcessingRules":true,
    "forwardTo":[
      {
        "emailAddress":{
          "name":"Alex Wilbur",
          "address":"AlexW@contoso.onmicrosoft.com"
        }
      }
    ]
  }
}
```



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
