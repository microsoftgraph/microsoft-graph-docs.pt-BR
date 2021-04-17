---
title: Obter userAttributeAssignments
description: Leia as propriedades e as relações de um objeto identityUserFlowAttributeAssignment.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: fa51cbdc0d58c9a80863eeb3743ca56ec9d2e890
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882768"
---
# <a name="get-identityuserflowattributeassignment"></a><span data-ttu-id="de997-103">Obter identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="de997-103">Get identityUserFlowAttributeAssignment</span></span>

<span data-ttu-id="de997-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de997-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="de997-105">Leia as propriedades e as relações de [um objeto identityUserFlowAttributeAssignment.](../resources/identityuserflowattributeassignment.md)</span><span class="sxs-lookup"><span data-stu-id="de997-105">Read the properties and relationships of an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="de997-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="de997-106">Permissions</span></span>

<span data-ttu-id="de997-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de997-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de997-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="de997-109">Permission type</span></span>|<span data-ttu-id="de997-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="de997-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de997-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="de997-111">Delegated (work or school account)</span></span>|<span data-ttu-id="de997-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de997-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="de997-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="de997-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de997-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="de997-114">Not supported</span></span>|
|<span data-ttu-id="de997-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="de997-115">Application</span></span>|<span data-ttu-id="de997-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de997-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="de997-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="de997-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="de997-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="de997-118">Optional query parameters</span></span>

<span data-ttu-id="de997-119">Este método dá suporte `$select` aos `$expand` parâmetros e de consulta para obter os detalhes do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="de997-119">This method supports the `$select` and `$expand` query parameters to get the details of the user flow attribute.</span></span> <span data-ttu-id="de997-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="de997-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="de997-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="de997-121">Request headers</span></span>

|<span data-ttu-id="de997-122">Nome</span><span class="sxs-lookup"><span data-stu-id="de997-122">Name</span></span>|<span data-ttu-id="de997-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="de997-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="de997-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="de997-124">Authorization</span></span>|<span data-ttu-id="de997-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="de997-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="de997-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="de997-127">Request body</span></span>

<span data-ttu-id="de997-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="de997-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de997-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="de997-129">Response</span></span>

<span data-ttu-id="de997-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="de997-130">If successful, this method returns a `200 OK` response code and an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="de997-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="de997-131">Examples</span></span>

### <a name="example-1-get-the-details-of-an-identityuserflowattributeassignment"></a><span data-ttu-id="de997-132">Exemplo 1: Obter os detalhes de uma identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="de997-132">Example 1: Get the details of an identityUserFlowAttributeAssignment</span></span>

#### <a name="request"></a><span data-ttu-id="de997-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de997-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment_3"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments/City
```

#### <a name="response"></a><span data-ttu-id="de997-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="de997-134">Response</span></span>

<span data-ttu-id="de997-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="de997-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows('userFlowId')/userAttributeAssignments/$entity",
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

### <a name="example-2-get-the-details-of-an-identityuserflowattributeassignment-and-expand-userattribute"></a><span data-ttu-id="de997-136">Exemplo 2: obter os detalhes de uma identityUserFlowAttributeAssignment e expandir userAttribute</span><span class="sxs-lookup"><span data-stu-id="de997-136">Example 2: Get the details of an identityUserFlowAttributeAssignment and expand userAttribute</span></span>

#### <a name="request"></a><span data-ttu-id="de997-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="de997-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment_expand_3"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/{id}/userAttributeAssignments/{id}?$expand=userAttribute
```

#### <a name="response"></a><span data-ttu-id="de997-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="de997-138">Response</span></span>

<span data-ttu-id="de997-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="de997-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows('userFlowId')/userAttributeAssignments/$entity",
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
