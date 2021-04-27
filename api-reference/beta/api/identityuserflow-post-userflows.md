---
title: Criar userFlow
description: Use essa API para criar um novo userFlow.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e05529179ce498d58857a0308fcd615866cf39ed
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040669"
---
# <a name="create-userflow"></a><span data-ttu-id="937b5-103">Criar userFlow</span><span class="sxs-lookup"><span data-stu-id="937b5-103">Create userFlow</span></span>

<span data-ttu-id="937b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="937b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="937b5-105">Crie um novo [objeto userFlow.](../resources/identityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="937b5-105">Create a new [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="937b5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="937b5-106">Permissions</span></span>

<span data-ttu-id="937b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="937b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="937b5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="937b5-109">Permission type</span></span>                        | <span data-ttu-id="937b5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="937b5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="937b5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="937b5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="937b5-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="937b5-112">IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="937b5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="937b5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="937b5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="937b5-114">Not supported.</span></span> |
| <span data-ttu-id="937b5-115">Application</span><span class="sxs-lookup"><span data-stu-id="937b5-115">Application</span></span>                            | <span data-ttu-id="937b5-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="937b5-116">IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="937b5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="937b5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/userFlows
```

## <a name="request-headers"></a><span data-ttu-id="937b5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="937b5-118">Request headers</span></span>

| <span data-ttu-id="937b5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="937b5-119">Name</span></span>          | <span data-ttu-id="937b5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="937b5-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="937b5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="937b5-121">Authorization</span></span> | <span data-ttu-id="937b5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="937b5-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="937b5-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="937b5-124">Content-type</span></span> | <span data-ttu-id="937b5-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="937b5-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="937b5-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="937b5-127">Request body</span></span>

<span data-ttu-id="937b5-128">No corpo da solicitação, fornece uma representação JSON do [objeto userFlow.](../resources/identityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="937b5-128">In the request body, supply a JSON representation of [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="937b5-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="937b5-129">Response</span></span>

<span data-ttu-id="937b5-130">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto userFlow](../resources/identityuserflow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="937b5-130">If successful, this method returns a `201 Created` response code and a new [userFlow](../resources/identityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="937b5-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="937b5-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="937b5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="937b5-132">Request</span></span>

<span data-ttu-id="937b5-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="937b5-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="937b5-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="937b5-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_identityuserflow_from_identitycontainer"
}-->

```http
POST https://graph.microsoft.com/beta/identity/userFlows
Content-type: application/json

{
  "id": "Pol1",
  "userFlowType": "signUpOrSignIn",
  "userFlowTypeVersion": 1
}
```
# <a name="c"></a>[<span data-ttu-id="937b5-135">C#</span><span class="sxs-lookup"><span data-stu-id="937b5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityuserflow-from-identitycontainer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="937b5-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="937b5-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityuserflow-from-identitycontainer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="937b5-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="937b5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityuserflow-from-identitycontainer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="937b5-138">Java</span><span class="sxs-lookup"><span data-stu-id="937b5-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityuserflow-from-identitycontainer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="937b5-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="937b5-139">Response</span></span>

<span data-ttu-id="937b5-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="937b5-140">The following is an example of the response.</span></span>

> <span data-ttu-id="937b5-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="937b5-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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


