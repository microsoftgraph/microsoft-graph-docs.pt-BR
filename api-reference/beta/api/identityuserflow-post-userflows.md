---
title: Criar userflow
description: Use esta API para criar um novo userflow.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fdc5266722b9dafd1067429a538be76d62493bf0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47990701"
---
# <a name="create-userflow"></a><span data-ttu-id="6268f-103">Criar userflow</span><span class="sxs-lookup"><span data-stu-id="6268f-103">Create userFlow</span></span>

<span data-ttu-id="6268f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6268f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6268f-105">Criar um novo objeto [userflow](../resources/identityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="6268f-105">Create a new [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6268f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6268f-106">Permissions</span></span>

<span data-ttu-id="6268f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6268f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6268f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6268f-109">Permission type</span></span>                        | <span data-ttu-id="6268f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6268f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6268f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6268f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6268f-112">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6268f-112">IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="6268f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6268f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6268f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6268f-114">Not supported.</span></span> |
| <span data-ttu-id="6268f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6268f-115">Application</span></span>                            | <span data-ttu-id="6268f-116">IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6268f-116">IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6268f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6268f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/userFlows
```

## <a name="request-headers"></a><span data-ttu-id="6268f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6268f-118">Request headers</span></span>

| <span data-ttu-id="6268f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6268f-119">Name</span></span>          | <span data-ttu-id="6268f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6268f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6268f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6268f-121">Authorization</span></span> | <span data-ttu-id="6268f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6268f-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="6268f-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="6268f-124">Content-type</span></span> | <span data-ttu-id="6268f-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6268f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6268f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6268f-127">Request body</span></span>

<span data-ttu-id="6268f-128">No corpo da solicitação, forneça uma representação JSON do objeto [userflow](../resources/identityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="6268f-128">In the request body, supply a JSON representation of [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6268f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6268f-129">Response</span></span>

<span data-ttu-id="6268f-130">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [userflow](../resources/identityuserflow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6268f-130">If successful, this method returns a `201 Created` response code and a new [userFlow](../resources/identityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6268f-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6268f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6268f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6268f-132">Request</span></span>

<span data-ttu-id="6268f-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6268f-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6268f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6268f-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6268f-135">C#</span><span class="sxs-lookup"><span data-stu-id="6268f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityuserflow-from-identitycontainer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6268f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6268f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityuserflow-from-identitycontainer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6268f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6268f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityuserflow-from-identitycontainer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6268f-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6268f-138">Response</span></span>

<span data-ttu-id="6268f-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6268f-139">The following is an example of the response.</span></span>

> <span data-ttu-id="6268f-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6268f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


