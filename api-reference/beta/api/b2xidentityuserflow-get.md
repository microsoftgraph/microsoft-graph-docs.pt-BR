---
title: Obter b2xIdentityUserFlow
description: Recupere as propriedades e os relacionamentos de um objeto b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5b32f8abb87892dcd1149a7614a921897e1b229c
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961081"
---
# <a name="get-b2xidentityuserflow"></a><span data-ttu-id="e8d11-103">Obter b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="e8d11-103">Get b2xIdentityUserFlow</span></span>

<span data-ttu-id="e8d11-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8d11-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8d11-105">Recupere as propriedades e os relacionamentos de um objeto [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="e8d11-105">Retrieve the properties and relationships of a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8d11-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e8d11-106">Permissions</span></span>

<span data-ttu-id="e8d11-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8d11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8d11-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8d11-109">Permission type</span></span>      | <span data-ttu-id="e8d11-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e8d11-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8d11-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8d11-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e8d11-112">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e8d11-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="e8d11-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8d11-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="e8d11-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8d11-114">Not supported.</span></span>|
|<span data-ttu-id="e8d11-115">Application</span><span class="sxs-lookup"><span data-stu-id="e8d11-115">Application</span></span>|<span data-ttu-id="e8d11-116">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e8d11-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="e8d11-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="e8d11-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="e8d11-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="e8d11-118">Global administrator</span></span>
* <span data-ttu-id="e8d11-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="e8d11-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="e8d11-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8d11-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8d11-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e8d11-121">Optional query parameters</span></span>

<span data-ttu-id="e8d11-122">Você pode usar o `$expand` para expandir Propriedades de fluxo de usuário específicas que não são expandidas por padrão.</span><span class="sxs-lookup"><span data-stu-id="e8d11-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span>

<span data-ttu-id="e8d11-123">Para obter mais informações, consulte [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="e8d11-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8d11-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8d11-124">Request headers</span></span>

|<span data-ttu-id="e8d11-125">Nome</span><span class="sxs-lookup"><span data-stu-id="e8d11-125">Name</span></span>|<span data-ttu-id="e8d11-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8d11-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="e8d11-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8d11-127">Authorization</span></span>|<span data-ttu-id="e8d11-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8d11-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8d11-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8d11-130">Request body</span></span>

<span data-ttu-id="e8d11-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8d11-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8d11-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8d11-132">Response</span></span>

<span data-ttu-id="e8d11-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma representação JSON do [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8d11-133">If successful, this method returns a `200 OK` response code and a JSON representation of the [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8d11-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8d11-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8d11-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8d11-135">Request</span></span>

<span data-ttu-id="e8d11-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8d11-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e8d11-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8d11-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="e8d11-138">C#</span><span class="sxs-lookup"><span data-stu-id="e8d11-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2xuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8d11-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8d11-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2xuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e8d11-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e8d11-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2xuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e8d11-141">Java</span><span class="sxs-lookup"><span data-stu-id="e8d11-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2xuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e8d11-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8d11-142">Response</span></span>

<span data-ttu-id="e8d11-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e8d11-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "B2X_1_PartnerSignUp",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Get b2xUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: get_b2xUserFlows/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->


