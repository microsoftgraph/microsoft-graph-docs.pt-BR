---
title: Obter userflow
description: Recupere as propriedades e os relacionamentos do objeto userflow.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ee9bedb3fd81d638e8e7d996e1d6afe9e8ce1c64
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938610"
---
# <a name="get-userflow"></a><span data-ttu-id="46ebe-103">Obter userflow</span><span class="sxs-lookup"><span data-stu-id="46ebe-103">Get userFlow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46ebe-104">Recupere as propriedades e associações de um objeto [userflow](../resources/identityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="46ebe-104">Retrieve the properties and associations for an [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="46ebe-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="46ebe-105">Permissions</span></span>

<span data-ttu-id="46ebe-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46ebe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="46ebe-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="46ebe-108">Permission type</span></span>                        | <span data-ttu-id="46ebe-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="46ebe-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="46ebe-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="46ebe-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="46ebe-111">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="46ebe-111">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="46ebe-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="46ebe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46ebe-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="46ebe-113">Not supported.</span></span> |
| <span data-ttu-id="46ebe-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="46ebe-114">Application</span></span>                            | <span data-ttu-id="46ebe-115">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="46ebe-115">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="46ebe-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="46ebe-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="46ebe-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="46ebe-117">Request headers</span></span>

| <span data-ttu-id="46ebe-118">Nome</span><span class="sxs-lookup"><span data-stu-id="46ebe-118">Name</span></span>      |<span data-ttu-id="46ebe-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="46ebe-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="46ebe-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="46ebe-120">Authorization</span></span> | <span data-ttu-id="46ebe-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46ebe-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="46ebe-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="46ebe-123">Content-type</span></span> | <span data-ttu-id="46ebe-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="46ebe-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="46ebe-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="46ebe-126">Request body</span></span>

<span data-ttu-id="46ebe-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="46ebe-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46ebe-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="46ebe-128">Response</span></span>

<span data-ttu-id="46ebe-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [userflow](../resources/identityuserflow.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="46ebe-129">If successful, this method returns a `200 OK` response code and the requested [userFlow](../resources/identityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="46ebe-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="46ebe-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="46ebe-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="46ebe-131">Request</span></span>

<span data-ttu-id="46ebe-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="46ebe-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="46ebe-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="46ebe-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityuserflow"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/userFlows/B2C_1_Pol1
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="46ebe-134">C#</span><span class="sxs-lookup"><span data-stu-id="46ebe-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="46ebe-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="46ebe-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="46ebe-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="46ebe-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="46ebe-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="46ebe-137">Response</span></span>

<span data-ttu-id="46ebe-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="46ebe-138">The following is an example of the response.</span></span>

> <span data-ttu-id="46ebe-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="46ebe-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.UserFlow"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "B2C_1_Pol1",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get UserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
   "suppressions": [
    "Error: get_identityuserflow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
