---
title: Listar userAttributeAssignments
description: Obter os recursos identityUserFlowAttributeAssignment da propriedade de navegação userAttributeAssignments em um b2cIdentityUserFlow.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 46a3f1d7c33440976a71b142b1ec5fc4616c26cf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944714"
---
# <a name="list-userattributeassignments"></a><span data-ttu-id="34299-103">Listar userAttributeAssignments</span><span class="sxs-lookup"><span data-stu-id="34299-103">List userAttributeAssignments</span></span>

<span data-ttu-id="34299-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34299-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="34299-105">Obter os recursos identityUserFlowAttributeAssignment da propriedade de navegação userAttributeAssignments em [um b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="34299-105">Get the identityUserFlowAttributeAssignment resources from the userAttributeAssignments navigation property in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="34299-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="34299-106">Permissions</span></span>

<span data-ttu-id="34299-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34299-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34299-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34299-109">Permission type</span></span>|<span data-ttu-id="34299-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="34299-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34299-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34299-111">Delegated (work or school account)</span></span>|<span data-ttu-id="34299-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34299-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="34299-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34299-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34299-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="34299-114">Not supported</span></span>|
|<span data-ttu-id="34299-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34299-115">Application</span></span>|<span data-ttu-id="34299-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34299-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="34299-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34299-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/userAttributeAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="34299-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="34299-118">Optional query parameters</span></span>

<span data-ttu-id="34299-119">Este método dá suporte `$select` aos `$expand` parâmetros e para obter os detalhes do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="34299-119">This method supports the `$select` and `$expand` parameters to get the details of the user flow attribute.</span></span> <span data-ttu-id="34299-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="34299-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="34299-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34299-121">Request headers</span></span>

|<span data-ttu-id="34299-122">Nome</span><span class="sxs-lookup"><span data-stu-id="34299-122">Name</span></span>|<span data-ttu-id="34299-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="34299-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="34299-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="34299-124">Authorization</span></span>|<span data-ttu-id="34299-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34299-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="34299-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34299-127">Request body</span></span>

<span data-ttu-id="34299-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="34299-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34299-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="34299-129">Response</span></span>

<span data-ttu-id="34299-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34299-130">If successful, this method returns a `200 OK` response code and a collection of [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="34299-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="34299-131">Examples</span></span>

### <a name="example-1-list-userattributeassignments-in-a-b2cidentityuserflow"></a><span data-ttu-id="34299-132">Exemplo 1: Listar userAttributeAssignments em um b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="34299-132">Example 1: List userAttributeAssignments in a b2cIdentityUserFlow</span></span>

#### <a name="request"></a><span data-ttu-id="34299-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34299-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="34299-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="34299-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment_1"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments?
```
# <a name="c"></a>[<span data-ttu-id="34299-135">C#</span><span class="sxs-lookup"><span data-stu-id="34299-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityuserflowattributeassignment-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="34299-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="34299-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityuserflowattributeassignment-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="34299-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="34299-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityuserflowattributeassignment-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="34299-138">Java</span><span class="sxs-lookup"><span data-stu-id="34299-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityuserflowattributeassignment-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="34299-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="34299-139">Response</span></span>

<span data-ttu-id="34299-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="34299-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.identityUserFlowAttributeAssignment)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.identityUserFlowAttributeAssignment",
    "value": [
        {
            "id": "City",
            "isOptional": false,
            "requiresVerification": false,
            "userInputType": "RadioSingleSelect",
            "displayName": "City",
            "userAttributeValues": [
                {
                    "name": "S",
                    "value": "1",
                    "isDefault": true
                }
            ]
        },
        {
            "id": "extension_guid_shoeSize",
            "isOptional": false,
            "requiresVerification": false,
            "userInputType": "TextBox",
            "displayName": "Shoe size",
            "userFlowId": "B2C_1_Consumer",
            "userAttributeValues": []
        }
    ]
}
```

### <a name="example-2-list-userattributeassignments-in-a-b2cidentityuserflow-and-expand-userattribute"></a><span data-ttu-id="34299-141">Exemplo 2: Listar userAttributeAssignments em um b2cIdentityUserFlow e expandir userAttribute</span><span class="sxs-lookup"><span data-stu-id="34299-141">Example 2: List userAttributeAssignments in a b2cIdentityUserFlow and expand userAttribute</span></span>

#### <a name="request"></a><span data-ttu-id="34299-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34299-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="34299-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="34299-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment_expand_1"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments?$expand=userAttribute
```
# <a name="c"></a>[<span data-ttu-id="34299-144">C#</span><span class="sxs-lookup"><span data-stu-id="34299-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityuserflowattributeassignment-expand-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="34299-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="34299-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityuserflowattributeassignment-expand-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="34299-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="34299-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityuserflowattributeassignment-expand-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="34299-147">Java</span><span class="sxs-lookup"><span data-stu-id="34299-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityuserflowattributeassignment-expand-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="34299-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="34299-148">Response</span></span>

<span data-ttu-id="34299-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="34299-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.identityUserFlowAttributeAssignment)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.identityUserFlowAttributeAssignment",
    "value": [
        {
            "id": "City",
            "isOptional": false,
            "requiresVerification": false,
            "userInputType": "RadioSingleSelect",
            "displayName": "City",
            "userAttributeValues": [
                {
                    "name": "S",
                    "value": "1",
                    "isDefault": true
                }
            ],
            "userAttribute": {
                "@odata.type": "#Microsoft.Graph.BuiltInUserFlowAttribute",
                "id": "City",
                "displayName": "City",
                "description": "your city",
                "userFlowAttributeType": "builtIn",
                "dataType": "string"
            }
        },
        {
            "id": "extension_guid_shoeSize",
            "isOptional": false,
            "requiresVerification": false,
            "userInputType": "TextBox",
            "displayName": "Shoe size",
            "userFlowId": "B2C_1_Consumer",
            "userAttributeValues": [],
            "userAttribute": {
                "@odata.type": "#Microsoft.Graph.CustomUserFlowAttribute",
                "id": "extension_guid_shoeSize",
                "displayName": "Shoe size",
                "description": "Your shoe size",
                "userFlowAttributeType": "custom",
                "dataType": "string"
            }
        }
    ]
}
```
