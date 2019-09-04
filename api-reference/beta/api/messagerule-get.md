---
title: Obter regra
description: Obtenha as propriedades e as relações de um objeto messageRule.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7aaf0be15e711fdc91cf4fabeaab77d238c1e38c
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726078"
---
# <a name="get-rule"></a><span data-ttu-id="ec551-103">Obter regra</span><span class="sxs-lookup"><span data-stu-id="ec551-103">Get rule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec551-104">Obtenha as propriedades e as relações de um objeto [messageRule](../resources/messagerule.md).</span><span class="sxs-lookup"><span data-stu-id="ec551-104">Get the properties and relationships of a [messageRule](../resources/messagerule.md) object.</span></span>


## <a name="permissions"></a><span data-ttu-id="ec551-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ec551-105">Permissions</span></span>
<span data-ttu-id="ec551-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec551-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec551-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec551-108">Permission type</span></span>      | <span data-ttu-id="ec551-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ec551-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec551-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec551-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ec551-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="ec551-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="ec551-112">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec551-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec551-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="ec551-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="ec551-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec551-114">Application</span></span> | <span data-ttu-id="ec551-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="ec551-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec551-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec551-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/inbox/messagerules/{id}
GET /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ec551-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ec551-117">Optional query parameters</span></span>
<span data-ttu-id="ec551-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ec551-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec551-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec551-119">Request headers</span></span>
| <span data-ttu-id="ec551-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ec551-120">Name</span></span>      |<span data-ttu-id="ec551-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec551-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ec551-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec551-122">Authorization</span></span>  | <span data-ttu-id="ec551-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec551-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="ec551-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec551-125">Request body</span></span>
<span data-ttu-id="ec551-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ec551-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ec551-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec551-127">Response</span></span>
<span data-ttu-id="ec551-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [messageRule](../resources/messagerule.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec551-128">If successful, this method returns a `200 OK` response code and [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ec551-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ec551-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec551-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec551-130">Request</span></span>
<span data-ttu-id="ec551-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec551-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ec551-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec551-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_messagerule"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ec551-133">C#</span><span class="sxs-lookup"><span data-stu-id="ec551-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ec551-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec551-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ec551-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ec551-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ec551-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec551-136">Response</span></span>
<span data-ttu-id="ec551-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec551-137">Here is an example of the response.</span></span> <span data-ttu-id="ec551-138">Por padrão, as propriedades de data e hora na resposta estão em UTC.</span><span class="sxs-lookup"><span data-stu-id="ec551-138">By default, the date-time properties in the response are in UTC.</span></span> 

<span data-ttu-id="ec551-p104">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec551-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
