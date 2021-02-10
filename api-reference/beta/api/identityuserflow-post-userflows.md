---
title: Criar userFlow
description: Use essa API para criar um novo userFlow.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 36ccf24fb65a0098ebccb8774c36af804aece41f
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176525"
---
# <a name="create-userflow"></a><span data-ttu-id="8ed6e-103">Criar userFlow</span><span class="sxs-lookup"><span data-stu-id="8ed6e-103">Create userFlow</span></span>

<span data-ttu-id="8ed6e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ed6e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ed6e-105">Criar um novo [objeto userFlow.](../resources/identityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="8ed6e-105">Create a new [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ed6e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8ed6e-106">Permissions</span></span>

<span data-ttu-id="8ed6e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ed6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8ed6e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8ed6e-109">Permission type</span></span>                        | <span data-ttu-id="8ed6e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8ed6e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8ed6e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8ed6e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8ed6e-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ed6e-112">IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="8ed6e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8ed6e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ed6e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8ed6e-114">Not supported.</span></span> |
| <span data-ttu-id="8ed6e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8ed6e-115">Application</span></span>                            | <span data-ttu-id="8ed6e-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ed6e-116">IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ed6e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8ed6e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identity/userFlows
```

## <a name="request-headers"></a><span data-ttu-id="8ed6e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8ed6e-118">Request headers</span></span>

| <span data-ttu-id="8ed6e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8ed6e-119">Name</span></span>          | <span data-ttu-id="8ed6e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ed6e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8ed6e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8ed6e-121">Authorization</span></span> | <span data-ttu-id="8ed6e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ed6e-p102">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="8ed6e-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="8ed6e-124">Content-type</span></span> | <span data-ttu-id="8ed6e-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8ed6e-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ed6e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8ed6e-127">Request body</span></span>

<span data-ttu-id="8ed6e-128">No corpo da solicitação, fornece uma representação JSON do [objeto userFlow.](../resources/identityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="8ed6e-128">In the request body, supply a JSON representation of [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8ed6e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ed6e-129">Response</span></span>

<span data-ttu-id="8ed6e-130">Se bem-sucedido, este método retorna `201 Created` um código de resposta e um novo objeto [userFlow](../resources/identityuserflow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8ed6e-130">If successful, this method returns a `201 Created` response code and a new [userFlow](../resources/identityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8ed6e-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8ed6e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8ed6e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8ed6e-132">Request</span></span>

<span data-ttu-id="8ed6e-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8ed6e-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8ed6e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8ed6e-134">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8ed6e-135">C#</span><span class="sxs-lookup"><span data-stu-id="8ed6e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-identityuserflow-from-identitycontainer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8ed6e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8ed6e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-identityuserflow-from-identitycontainer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8ed6e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8ed6e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-identityuserflow-from-identitycontainer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8ed6e-138">Java</span><span class="sxs-lookup"><span data-stu-id="8ed6e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-identityuserflow-from-identitycontainer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8ed6e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="8ed6e-139">Response</span></span>

<span data-ttu-id="8ed6e-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8ed6e-140">The following is an example of the response.</span></span>

> <span data-ttu-id="8ed6e-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8ed6e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


