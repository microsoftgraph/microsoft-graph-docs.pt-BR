---
title: Listar transflows
description: Recupere uma lista de objetos userflow.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f35437e30768600277f505e43cc35517d2cf32af
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47990722"
---
# <a name="list-userflows"></a><span data-ttu-id="e8a48-103">Listar transflows</span><span class="sxs-lookup"><span data-stu-id="e8a48-103">List userFlows</span></span>

<span data-ttu-id="e8a48-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8a48-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8a48-105">Recupere uma lista de [userflows](../resources/identityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="e8a48-105">Retrieve a list of [userflows](../resources/identityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e8a48-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8a48-106">Permissions</span></span>

<span data-ttu-id="e8a48-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8a48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e8a48-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8a48-109">Permission type</span></span>                        | <span data-ttu-id="e8a48-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8a48-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e8a48-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8a48-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e8a48-112">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e8a48-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>  |
| <span data-ttu-id="e8a48-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8a48-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8a48-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8a48-114">Not supported.</span></span> |
| <span data-ttu-id="e8a48-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8a48-115">Application</span></span>                            | <span data-ttu-id="e8a48-116">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e8a48-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8a48-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8a48-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlows
```

## <a name="request-headers"></a><span data-ttu-id="e8a48-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8a48-118">Request headers</span></span>

| <span data-ttu-id="e8a48-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e8a48-119">Name</span></span>      |<span data-ttu-id="e8a48-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8a48-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e8a48-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8a48-121">Authorization</span></span> | <span data-ttu-id="e8a48-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8a48-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8a48-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8a48-124">Request body</span></span>

<span data-ttu-id="e8a48-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8a48-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8a48-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8a48-126">Response</span></span>

<span data-ttu-id="e8a48-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [userflow](../resources/identityuserflow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8a48-127">If successful, this method returns a `200 OK` response code and a collection of [userFlow](../resources/identityuserflow.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e8a48-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e8a48-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e8a48-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8a48-129">Request</span></span>

<span data-ttu-id="e8a48-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8a48-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e8a48-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8a48-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflows"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/userFlows
```
# <a name="c"></a>[<span data-ttu-id="e8a48-132">C#</span><span class="sxs-lookup"><span data-stu-id="e8a48-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8a48-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8a48-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8a48-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8a48-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e8a48-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8a48-135">Response</span></span>

<span data-ttu-id="e8a48-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e8a48-136">The following is an example of the response.</span></span>

> <span data-ttu-id="e8a48-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8a48-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


