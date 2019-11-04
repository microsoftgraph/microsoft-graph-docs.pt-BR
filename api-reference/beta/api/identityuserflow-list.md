---
title: Listar transflows
description: Recupere uma lista de objetos userflow.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 585353891219f47666b980a532cd8a7d3dea3918
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938580"
---
# <a name="list-userflows"></a><span data-ttu-id="a6f32-103">Listar transflows</span><span class="sxs-lookup"><span data-stu-id="a6f32-103">List userFlows</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6f32-104">Recupere uma lista de [userflows](../resources/identityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="a6f32-104">Retrieve a list of [userflows](../resources/identityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a6f32-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a6f32-105">Permissions</span></span>

<span data-ttu-id="a6f32-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6f32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a6f32-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6f32-108">Permission type</span></span>                        | <span data-ttu-id="a6f32-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6f32-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a6f32-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6f32-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6f32-111">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a6f32-111">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>  |
| <span data-ttu-id="a6f32-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6f32-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6f32-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6f32-113">Not supported.</span></span> |
| <span data-ttu-id="a6f32-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6f32-114">Application</span></span>                            | <span data-ttu-id="a6f32-115">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="a6f32-115">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6f32-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6f32-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlows
```

## <a name="request-headers"></a><span data-ttu-id="a6f32-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6f32-117">Request headers</span></span>

| <span data-ttu-id="a6f32-118">Nome</span><span class="sxs-lookup"><span data-stu-id="a6f32-118">Name</span></span>      |<span data-ttu-id="a6f32-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6f32-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a6f32-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6f32-120">Authorization</span></span> | <span data-ttu-id="a6f32-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6f32-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6f32-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6f32-123">Request body</span></span>

<span data-ttu-id="a6f32-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a6f32-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6f32-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6f32-125">Response</span></span>

<span data-ttu-id="a6f32-126">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [userflow](../resources/identityuserflow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6f32-126">If successful, this method returns a `200 OK` response code and a collection of [userFlow](../resources/identityuserflow.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a6f32-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a6f32-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a6f32-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6f32-128">Request</span></span>

<span data-ttu-id="a6f32-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6f32-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a6f32-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6f32-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflows"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/userFlows
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a6f32-131">C#</span><span class="sxs-lookup"><span data-stu-id="a6f32-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a6f32-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6f32-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a6f32-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6f32-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a6f32-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6f32-134">Response</span></span>

<span data-ttu-id="a6f32-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a6f32-135">The following is an example of the response.</span></span>

> <span data-ttu-id="a6f32-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6f32-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.UserFlow",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "B2C_1_UserFlow1",
      "userFlowType": "signUpOrSignIn",
      "userFlowTypeVersion": 1
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List userFlows",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: get_userflows/container/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
