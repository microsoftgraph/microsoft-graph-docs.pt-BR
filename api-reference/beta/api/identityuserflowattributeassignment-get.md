---
title: Obter userAttributeAssignments
description: Leia as propriedades e as relações de um objeto identityUserFlowAttributeAssignment.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ec932b01dfae55dd9958063fccc57e99be9b3958
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435155"
---
# <a name="get-identityuserflowattributeassignment"></a><span data-ttu-id="37d70-103">Obter identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="37d70-103">Get identityUserFlowAttributeAssignment</span></span>

<span data-ttu-id="37d70-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37d70-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="37d70-105">Leia as propriedades e as relações de [um objeto identityUserFlowAttributeAssignment.](../resources/identityuserflowattributeassignment.md)</span><span class="sxs-lookup"><span data-stu-id="37d70-105">Read the properties and relationships of an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="37d70-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="37d70-106">Permissions</span></span>

<span data-ttu-id="37d70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37d70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37d70-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="37d70-109">Permission type</span></span>|<span data-ttu-id="37d70-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="37d70-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37d70-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="37d70-111">Delegated (work or school account)</span></span>|<span data-ttu-id="37d70-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37d70-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="37d70-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="37d70-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37d70-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="37d70-114">Not supported</span></span>|
|<span data-ttu-id="37d70-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="37d70-115">Application</span></span>|<span data-ttu-id="37d70-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37d70-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="37d70-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="37d70-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
GET /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="37d70-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="37d70-118">Optional query parameters</span></span>

<span data-ttu-id="37d70-119">Este método dá suporte `$select` aos `$expand` parâmetros e de consulta para obter os detalhes do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="37d70-119">This method supports the `$select` and `$expand` query parameters to get the details of the user flow attribute.</span></span> <span data-ttu-id="37d70-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="37d70-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="37d70-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="37d70-121">Request headers</span></span>

|<span data-ttu-id="37d70-122">Nome</span><span class="sxs-lookup"><span data-stu-id="37d70-122">Name</span></span>|<span data-ttu-id="37d70-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="37d70-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="37d70-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="37d70-124">Authorization</span></span>|<span data-ttu-id="37d70-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="37d70-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="37d70-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="37d70-127">Request body</span></span>

<span data-ttu-id="37d70-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="37d70-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37d70-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="37d70-129">Response</span></span>

<span data-ttu-id="37d70-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="37d70-130">If successful, this method returns a `200 OK` response code and an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="37d70-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="37d70-131">Examples</span></span>

### <a name="example-1-get-the-details-of-an-identityuserflowattributeassignment"></a><span data-ttu-id="37d70-132">Exemplo 1: Obter os detalhes de uma identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="37d70-132">Example 1: Get the details of an identityUserFlowAttributeAssignment</span></span>

#### <a name="request"></a><span data-ttu-id="37d70-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37d70-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="37d70-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="37d70-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
```
# <a name="c"></a>[<span data-ttu-id="37d70-135">C#</span><span class="sxs-lookup"><span data-stu-id="37d70-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityuserflowattributeassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37d70-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37d70-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityuserflowattributeassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37d70-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37d70-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityuserflowattributeassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37d70-138">Java</span><span class="sxs-lookup"><span data-stu-id="37d70-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityuserflowattributeassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="37d70-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="37d70-139">Response</span></span>

<span data-ttu-id="37d70-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="37d70-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('userFlowId')/userAttributeAssignments/$entity",
    "id": "City",
    "isOptional": false,
    "requiresVerification": false,
    "userInputType": "TextBox",
    "displayName": "City",
    "userAttributeValues": [
        {
            "name": "S",
            "value": "1",
            "isDefault": true
        }
    ]
}
```

### <a name="example-2-get-the-details-of-an-identityuserflowattributeassignment-and-expand-userattribute"></a><span data-ttu-id="37d70-141">Exemplo 2: obter os detalhes de uma identityUserFlowAttributeAssignment e expandir userAttribute</span><span class="sxs-lookup"><span data-stu-id="37d70-141">Example 2: Get the details of an identityUserFlowAttributeAssignment and expand userAttribute</span></span>

#### <a name="request"></a><span data-ttu-id="37d70-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="37d70-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="37d70-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="37d70-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment_expand"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/{id}?$expand=userAttribute
```
# <a name="c"></a>[<span data-ttu-id="37d70-144">C#</span><span class="sxs-lookup"><span data-stu-id="37d70-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityuserflowattributeassignment-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37d70-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37d70-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityuserflowattributeassignment-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37d70-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37d70-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityuserflowattributeassignment-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37d70-147">Java</span><span class="sxs-lookup"><span data-stu-id="37d70-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityuserflowattributeassignment-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="37d70-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="37d70-148">Response</span></span>

<span data-ttu-id="37d70-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="37d70-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('userFlowId')/userAttributeAssignments/$entity",
    "id": "City",
    "isOptional": false,
    "requiresVerification": false,
    "userInputType": "TextBox",
    "displayName": "City",
    "userAttributeValues": [
        {
            "name": "S",
            "value": "1",
            "isDefault": true
        }
    ],
    "userAttribute": {
        "id": "City",
        "displayName": "City",
        "description": "Your city",
        "userFlowAttributeType": "builtIn",
        "dataType": "string"
  }
}
```
