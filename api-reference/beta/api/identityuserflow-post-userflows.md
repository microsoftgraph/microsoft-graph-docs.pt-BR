---
title: Criar userflow
description: Use esta API para criar um novo userflow.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1cd660e4be738469351e3d1369d557774895ac58
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938552"
---
# <a name="create-userflow"></a><span data-ttu-id="02c1a-103">Criar userflow</span><span class="sxs-lookup"><span data-stu-id="02c1a-103">Create userFlow</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02c1a-104">Criar um novo objeto [userflow](../resources/identityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="02c1a-104">Create a new [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="02c1a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="02c1a-105">Permissions</span></span>

<span data-ttu-id="02c1a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02c1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="02c1a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02c1a-108">Permission type</span></span>                        | <span data-ttu-id="02c1a-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="02c1a-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="02c1a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02c1a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="02c1a-111">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="02c1a-111">IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="02c1a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02c1a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02c1a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02c1a-113">Not supported.</span></span> |
| <span data-ttu-id="02c1a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02c1a-114">Application</span></span>                            | <span data-ttu-id="02c1a-115">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="02c1a-115">IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02c1a-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02c1a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/userFlows
```

## <a name="request-headers"></a><span data-ttu-id="02c1a-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02c1a-117">Request headers</span></span>

| <span data-ttu-id="02c1a-118">Nome</span><span class="sxs-lookup"><span data-stu-id="02c1a-118">Name</span></span>          | <span data-ttu-id="02c1a-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="02c1a-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="02c1a-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="02c1a-120">Authorization</span></span> | <span data-ttu-id="02c1a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02c1a-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="02c1a-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="02c1a-123">Content-type</span></span> | <span data-ttu-id="02c1a-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02c1a-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02c1a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02c1a-126">Request body</span></span>

<span data-ttu-id="02c1a-127">No corpo da solicitação, forneça uma representação JSON do objeto [userflow](../resources/identityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="02c1a-127">In the request body, supply a JSON representation of [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="02c1a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="02c1a-128">Response</span></span>

<span data-ttu-id="02c1a-129">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [userflow](../resources/identityuserflow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02c1a-129">If successful, this method returns a `201 Created` response code and a new [userFlow](../resources/identityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="02c1a-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="02c1a-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="02c1a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02c1a-131">Request</span></span>

<span data-ttu-id="02c1a-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="02c1a-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="02c1a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="02c1a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_identityuserflow_from_identitycontainer"
}-->

```http
POST https://graph.microsoft.com/beta/identity/userFlows
Content-type: application/json

{
  "userFlowType": "signUpOrSignIn",
  "userFlowTypeVersion": 1
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="02c1a-134">C#</span><span class="sxs-lookup"><span data-stu-id="02c1a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityuserflow-from-identitycontainer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="02c1a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="02c1a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityuserflow-from-identitycontainer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="02c1a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="02c1a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityuserflow-from-identitycontainer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="02c1a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="02c1a-137">Response</span></span>

<span data-ttu-id="02c1a-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="02c1a-138">The following is an example of the response.</span></span>

> <span data-ttu-id="02c1a-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02c1a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.UserFlow"
} -->

```http
HTTP/1.1 201 Created
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
  "description": "Create UserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: create_identityuserflow_from_identitycontainer/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
