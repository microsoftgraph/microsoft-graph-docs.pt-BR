---
title: Obter b2xIdentityUserFlow
description: Recupere as propriedades e as relações de um objeto b2xIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 004c56043fa26f4141c029b64c88407feb2446bf
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438124"
---
# <a name="get-b2xidentityuserflow"></a><span data-ttu-id="4b53f-103">Obter b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="4b53f-103">Get b2xIdentityUserFlow</span></span>

<span data-ttu-id="4b53f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b53f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b53f-105">Recupere as propriedades e as relações de um [objeto b2xIdentityUserFlow.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="4b53f-105">Retrieve the properties and relationships of a [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4b53f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4b53f-106">Permissions</span></span>

<span data-ttu-id="4b53f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4b53f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b53f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4b53f-109">Permission type</span></span>      | <span data-ttu-id="4b53f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4b53f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4b53f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4b53f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4b53f-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b53f-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="4b53f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4b53f-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="4b53f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4b53f-114">Not supported.</span></span>|
|<span data-ttu-id="4b53f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4b53f-115">Application</span></span>|<span data-ttu-id="4b53f-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b53f-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="4b53f-117">A conta de trabalho ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="4b53f-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="4b53f-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="4b53f-118">Global administrator</span></span>
* <span data-ttu-id="4b53f-119">Administrador de Fluxo de Usuário de Identidade Externa</span><span class="sxs-lookup"><span data-stu-id="4b53f-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="4b53f-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4b53f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2xUserFlows/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4b53f-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4b53f-121">Optional query parameters</span></span>

<span data-ttu-id="4b53f-122">Você pode usar para expandir propriedades de fluxo de usuário `$expand` específicas que não são expandidas por padrão.</span><span class="sxs-lookup"><span data-stu-id="4b53f-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span>

<span data-ttu-id="4b53f-123">Para obter mais informações, consulte [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4b53f-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4b53f-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4b53f-124">Request headers</span></span>

|<span data-ttu-id="4b53f-125">Nome</span><span class="sxs-lookup"><span data-stu-id="4b53f-125">Name</span></span>|<span data-ttu-id="4b53f-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b53f-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="4b53f-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="4b53f-127">Authorization</span></span>|<span data-ttu-id="4b53f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4b53f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b53f-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4b53f-130">Request body</span></span>

<span data-ttu-id="4b53f-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4b53f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4b53f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b53f-132">Response</span></span>

<span data-ttu-id="4b53f-133">Se tiver êxito, este método retornará um código de resposta e uma representação JSON do `200 OK` [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4b53f-133">If successful, this method returns a `200 OK` response code and a JSON representation of the [b2xIdentityUserFlow](../resources/b2xidentityuserflow.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b53f-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b53f-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b53f-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b53f-135">Request</span></span>

<span data-ttu-id="4b53f-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4b53f-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4b53f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="4b53f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="4b53f-138">C#</span><span class="sxs-lookup"><span data-stu-id="4b53f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2xuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4b53f-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4b53f-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2xuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4b53f-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4b53f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2xuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4b53f-141">Java</span><span class="sxs-lookup"><span data-stu-id="4b53f-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2xuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4b53f-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="4b53f-142">Response</span></span>

<span data-ttu-id="4b53f-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4b53f-143">The following is an example of the response.</span></span>

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


