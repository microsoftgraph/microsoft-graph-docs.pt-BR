---
title: Obter userAttributeAssignments
description: Leia as propriedades e os relacionamentos de um objeto identityUserFlowAttributeAssignment.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c134e5e101080c007a0927fd18887262b8e10539
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581299"
---
# <a name="get-identityuserflowattributeassignment"></a><span data-ttu-id="4805c-103">Obter identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="4805c-103">Get identityUserFlowAttributeAssignment</span></span>

<span data-ttu-id="4805c-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="4805c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4805c-105">Leia as propriedades e os relacionamentos de um objeto [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="4805c-105">Read the properties and relationships of an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4805c-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="4805c-106">Permissions</span></span>

<span data-ttu-id="4805c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4805c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4805c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4805c-109">Permission type</span></span>|<span data-ttu-id="4805c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4805c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4805c-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4805c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4805c-112">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4805c-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="4805c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4805c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4805c-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="4805c-114">Not supported</span></span>|
|<span data-ttu-id="4805c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4805c-115">Application</span></span>|<span data-ttu-id="4805c-116">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="4805c-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4805c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4805c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
GET /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4805c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4805c-118">Optional query parameters</span></span>

<span data-ttu-id="4805c-119">Este método oferece suporte `$select` aos `$expand` parâmetros de consulta e para obter os detalhes do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="4805c-119">This method supports the `$select` and `$expand` query parameters to get the details of the user flow attribute.</span></span> <span data-ttu-id="4805c-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="4805c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4805c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4805c-121">Request headers</span></span>

|<span data-ttu-id="4805c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="4805c-122">Name</span></span>|<span data-ttu-id="4805c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4805c-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4805c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="4805c-124">Authorization</span></span>|<span data-ttu-id="4805c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4805c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4805c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4805c-127">Request body</span></span>

<span data-ttu-id="4805c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4805c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4805c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4805c-129">Response</span></span>

<span data-ttu-id="4805c-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4805c-130">If successful, this method returns a `200 OK` response code and an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4805c-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4805c-131">Examples</span></span>

### <a name="example-1-get-the-details-of-an-identityuserflowattributeassignment"></a><span data-ttu-id="4805c-132">Exemplo 1: obter os detalhes de um identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="4805c-132">Example 1: Get the details of an identityUserFlowAttributeAssignment</span></span>

#### <a name="request"></a><span data-ttu-id="4805c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4805c-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
```

#### <a name="response"></a><span data-ttu-id="4805c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4805c-134">Response</span></span>

<span data-ttu-id="4805c-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4805c-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-the-details-of-an-identityuserflowattributeassignment-and-expand-userattribute"></a><span data-ttu-id="4805c-136">Exemplo 2: obter os detalhes de um identityUserFlowAttributeAssignment e expandir userattribute</span><span class="sxs-lookup"><span data-stu-id="4805c-136">Example 2: Get the details of an identityUserFlowAttributeAssignment and expand userAttribute</span></span>

#### <a name="request"></a><span data-ttu-id="4805c-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4805c-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment_expand"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/{id}?$expand=userAttribute
```

#### <a name="response"></a><span data-ttu-id="4805c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4805c-138">Response</span></span>

<span data-ttu-id="4805c-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4805c-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
