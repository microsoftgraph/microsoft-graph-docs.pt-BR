---
title: Obter userflow
description: Recupere as propriedades e os relacionamentos do objeto userflow.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: aca28a2aaf1b659ef46537e53563b87236d558d0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47990736"
---
# <a name="get-userflow"></a><span data-ttu-id="6fd26-103">Obter userflow</span><span class="sxs-lookup"><span data-stu-id="6fd26-103">Get userFlow</span></span>

<span data-ttu-id="6fd26-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fd26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fd26-105">Recupere as propriedades e associações de um objeto [userflow](../resources/identityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="6fd26-105">Retrieve the properties and associations for an [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6fd26-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6fd26-106">Permissions</span></span>

<span data-ttu-id="6fd26-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6fd26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6fd26-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6fd26-109">Permission type</span></span>                        | <span data-ttu-id="6fd26-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6fd26-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6fd26-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6fd26-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6fd26-112">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6fd26-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="6fd26-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6fd26-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6fd26-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6fd26-114">Not supported.</span></span> |
| <span data-ttu-id="6fd26-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6fd26-115">Application</span></span>                            | <span data-ttu-id="6fd26-116">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="6fd26-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6fd26-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6fd26-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6fd26-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6fd26-118">Request headers</span></span>

| <span data-ttu-id="6fd26-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6fd26-119">Name</span></span>      |<span data-ttu-id="6fd26-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6fd26-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6fd26-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6fd26-121">Authorization</span></span> | <span data-ttu-id="6fd26-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6fd26-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6fd26-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="6fd26-124">Content-type</span></span> | <span data-ttu-id="6fd26-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6fd26-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6fd26-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6fd26-127">Request body</span></span>

<span data-ttu-id="6fd26-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6fd26-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6fd26-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fd26-129">Response</span></span>

<span data-ttu-id="6fd26-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto [userflow](../resources/identityuserflow.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6fd26-130">If successful, this method returns a `200 OK` response code and the requested [userFlow](../resources/identityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6fd26-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6fd26-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6fd26-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6fd26-132">Request</span></span>

<span data-ttu-id="6fd26-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6fd26-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6fd26-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6fd26-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityuserflow"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/userFlows/B2C_1_Pol1
```
# <a name="c"></a>[<span data-ttu-id="6fd26-135">C#</span><span class="sxs-lookup"><span data-stu-id="6fd26-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6fd26-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fd26-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6fd26-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6fd26-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6fd26-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="6fd26-138">Response</span></span>

<span data-ttu-id="6fd26-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6fd26-139">The following is an example of the response.</span></span>

> <span data-ttu-id="6fd26-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6fd26-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


