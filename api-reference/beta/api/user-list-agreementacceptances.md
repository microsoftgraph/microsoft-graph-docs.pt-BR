---
title: Listar agreementAcceptances
description: Recupere uma lista de objetos agreementAcceptance de um usuário.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5670f2da80169ac717d94443180c7fd13cb38592
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36724292"
---
# <a name="list-agreementacceptances"></a><span data-ttu-id="5a91f-103">Listar agreementAcceptances</span><span class="sxs-lookup"><span data-stu-id="5a91f-103">List agreementAcceptances</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a91f-104">Recupere uma lista de objetos [agreementAcceptance](../resources/agreementacceptance.md) de um usuário.</span><span class="sxs-lookup"><span data-stu-id="5a91f-104">Retrieve a list of a user's [agreementAcceptance](../resources/agreementacceptance.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="5a91f-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5a91f-105">Permissions</span></span>
<span data-ttu-id="5a91f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a91f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a91f-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a91f-108">Permission type</span></span>                        | <span data-ttu-id="5a91f-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5a91f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a91f-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a91f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5a91f-111">AgreementAcceptance.Read</span><span class="sxs-lookup"><span data-stu-id="5a91f-111">AgreementAcceptance.Read</span></span> |
|<span data-ttu-id="5a91f-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a91f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a91f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a91f-113">Not supported.</span></span> |
|<span data-ttu-id="5a91f-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a91f-114">Application</span></span>                            | <span data-ttu-id="5a91f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a91f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a91f-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a91f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/agreementAcceptances
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="5a91f-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a91f-117">Request headers</span></span>
| <span data-ttu-id="5a91f-118">Nome</span><span class="sxs-lookup"><span data-stu-id="5a91f-118">Name</span></span>      |<span data-ttu-id="5a91f-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a91f-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5a91f-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a91f-120">Authorization</span></span> | <span data-ttu-id="5a91f-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="5a91f-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a91f-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a91f-122">Request body</span></span>
<span data-ttu-id="5a91f-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5a91f-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5a91f-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a91f-124">Response</span></span>
<span data-ttu-id="5a91f-125">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [agreementAcceptance](../resources/agreementacceptance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a91f-125">If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5a91f-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a91f-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a91f-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a91f-127">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5a91f-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a91f-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptances"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5a91f-129">C#</span><span class="sxs-lookup"><span data-stu-id="5a91f-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreementacceptances-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5a91f-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a91f-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreementacceptances-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5a91f-131">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="5a91f-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreementacceptances-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5a91f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a91f-132">Response</span></span>
><span data-ttu-id="5a91f-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5a91f-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementAcceptance",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 303

{
  "value": [
    {
      "agreementId": "agreementId-value",
      "userId": "userId-value",
      "agreementFileId": "agreementFileId-value",
      "recordedDateTime": "datetime-value",
      "userDisplayName": "userDisplayName-value",
      "userPrincipalName": "userPrincipalName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List agreementAcceptances",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
