---
title: Obter userFlow
description: Recupere as propriedades e as relações do objeto userflow.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6f671cc351675dfb2f62bfe3ad992facd8def402
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040767"
---
# <a name="get-userflow"></a><span data-ttu-id="81007-103">Obter userFlow</span><span class="sxs-lookup"><span data-stu-id="81007-103">Get userFlow</span></span>

<span data-ttu-id="81007-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81007-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81007-105">Recupere as propriedades e associações de um [objeto userFlow.](../resources/identityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="81007-105">Retrieve the properties and associations for an [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="81007-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="81007-106">Permissions</span></span>

<span data-ttu-id="81007-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81007-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="81007-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81007-109">Permission type</span></span>                        | <span data-ttu-id="81007-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="81007-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="81007-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81007-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="81007-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81007-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="81007-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81007-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81007-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81007-114">Not supported.</span></span> |
| <span data-ttu-id="81007-115">Application</span><span class="sxs-lookup"><span data-stu-id="81007-115">Application</span></span>                            | <span data-ttu-id="81007-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81007-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="81007-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81007-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="81007-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81007-118">Request headers</span></span>

| <span data-ttu-id="81007-119">Nome</span><span class="sxs-lookup"><span data-stu-id="81007-119">Name</span></span>      |<span data-ttu-id="81007-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="81007-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="81007-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="81007-121">Authorization</span></span> | <span data-ttu-id="81007-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81007-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="81007-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="81007-124">Content-type</span></span> | <span data-ttu-id="81007-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81007-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81007-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81007-127">Request body</span></span>

<span data-ttu-id="81007-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="81007-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81007-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="81007-129">Response</span></span>

<span data-ttu-id="81007-130">Se tiver êxito, este método retornará um código `200 OK` de resposta e o objeto [userFlow](../resources/identityuserflow.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81007-130">If successful, this method returns a `200 OK` response code and the requested [userFlow](../resources/identityuserflow.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="81007-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="81007-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="81007-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81007-132">Request</span></span>

<span data-ttu-id="81007-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="81007-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="81007-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="81007-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityuserflow"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/userFlows/B2C_1_Pol1
```
# <a name="c"></a>[<span data-ttu-id="81007-135">C#</span><span class="sxs-lookup"><span data-stu-id="81007-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81007-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81007-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81007-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81007-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="81007-138">Java</span><span class="sxs-lookup"><span data-stu-id="81007-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityuserflow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="81007-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="81007-139">Response</span></span>

<span data-ttu-id="81007-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="81007-140">The following is an example of the response.</span></span>

> <span data-ttu-id="81007-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="81007-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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


