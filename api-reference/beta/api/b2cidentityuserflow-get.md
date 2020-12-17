---
title: Obter b2cIdentityUserFlow
description: Recupere as propriedades e os relacionamentos de um objeto b2cIdentityUserFlow.
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 45fc991d02a5b588f924154a8e9c4e639546f485
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49705713"
---
# <a name="get-b2cidentityuserflow"></a><span data-ttu-id="cd5ea-103">Obter b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="cd5ea-103">Get b2cIdentityUserFlow</span></span>

<span data-ttu-id="cd5ea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd5ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd5ea-105">Recupere as propriedades e os relacionamentos de um objeto [b2cUserFlow](../resources/b2cidentityuserflow.md) .</span><span class="sxs-lookup"><span data-stu-id="cd5ea-105">Retrieve the properties and relationships of a [b2cUserFlow](../resources/b2cidentityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd5ea-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cd5ea-106">Permissions</span></span>

<span data-ttu-id="cd5ea-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd5ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd5ea-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd5ea-109">Permission type</span></span>      | <span data-ttu-id="cd5ea-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cd5ea-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd5ea-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd5ea-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cd5ea-112">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="cd5ea-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="cd5ea-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd5ea-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="cd5ea-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd5ea-114">Not supported.</span></span>|
|<span data-ttu-id="cd5ea-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd5ea-115">Application</span></span>|<span data-ttu-id="cd5ea-116">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="cd5ea-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="cd5ea-117">A conta corporativa ou de estudante precisa pertencer a uma das seguintes funções:</span><span class="sxs-lookup"><span data-stu-id="cd5ea-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="cd5ea-118">Administrador global</span><span class="sxs-lookup"><span data-stu-id="cd5ea-118">Global administrator</span></span>
* <span data-ttu-id="cd5ea-119">Administrador de fluxo de usuário de identidade externa</span><span class="sxs-lookup"><span data-stu-id="cd5ea-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="cd5ea-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd5ea-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2cUserFlows/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cd5ea-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cd5ea-121">Optional query parameters</span></span>

<span data-ttu-id="cd5ea-122">Você pode usar o `$expand` para expandir Propriedades de fluxo de usuário específicas que não são expandidas por padrão.</span><span class="sxs-lookup"><span data-stu-id="cd5ea-122">You can use `$expand` to expand specific user flow properties that are not expanded by default.</span></span>

<span data-ttu-id="cd5ea-123">Para obter mais informações, consulte [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="cd5ea-123">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cd5ea-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd5ea-124">Request headers</span></span>

|<span data-ttu-id="cd5ea-125">Nome</span><span class="sxs-lookup"><span data-stu-id="cd5ea-125">Name</span></span>|<span data-ttu-id="cd5ea-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd5ea-126">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="cd5ea-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd5ea-127">Authorization</span></span>|<span data-ttu-id="cd5ea-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd5ea-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd5ea-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd5ea-130">Request body</span></span>

<span data-ttu-id="cd5ea-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cd5ea-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd5ea-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd5ea-132">Response</span></span>

<span data-ttu-id="cd5ea-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma representação JSON do [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cd5ea-133">If successful, this method returns a `200 OK` response code and a JSON representation of the [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd5ea-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cd5ea-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd5ea-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd5ea-135">Request</span></span>

<span data-ttu-id="cd5ea-136">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd5ea-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="cd5ea-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd5ea-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2cUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="cd5ea-138">C#</span><span class="sxs-lookup"><span data-stu-id="cd5ea-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd5ea-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd5ea-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd5ea-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd5ea-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cd5ea-141">Java</span><span class="sxs-lookup"><span data-stu-id="cd5ea-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2cuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cd5ea-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd5ea-142">Response</span></span>

<span data-ttu-id="cd5ea-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cd5ea-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "B2C_1_CustomerSignUp",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1,
    "isLanguageCustomizationEnabled": false,
    "defaultLanguageTag": null
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Get b2cUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: get_b2cUserFlows/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->


