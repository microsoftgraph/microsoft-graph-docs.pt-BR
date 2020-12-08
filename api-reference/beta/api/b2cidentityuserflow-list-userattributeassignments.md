---
title: Listar userAttributeAssignments
description: Obtenha os recursos identityUserFlowAttributeAssignment da propriedade de navegação userAttributeAssignments em um b2cIdentityUserFlow.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5a509725149545e43e0fe87026dc9a3b3fd4f05e
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581278"
---
# <a name="list-userattributeassignments"></a><span data-ttu-id="2bf53-103">Listar userAttributeAssignments</span><span class="sxs-lookup"><span data-stu-id="2bf53-103">List userAttributeAssignments</span></span>

<span data-ttu-id="2bf53-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2bf53-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2bf53-105">Obtenha os recursos identityUserFlowAttributeAssignment da propriedade de navegação userAttributeAssignments em um [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="2bf53-105">Get the identityUserFlowAttributeAssignment resources from the userAttributeAssignments navigation property in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2bf53-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="2bf53-106">Permissions</span></span>

<span data-ttu-id="2bf53-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bf53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bf53-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2bf53-109">Permission type</span></span>|<span data-ttu-id="2bf53-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2bf53-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bf53-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2bf53-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2bf53-112">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2bf53-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="2bf53-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2bf53-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bf53-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="2bf53-114">Not supported</span></span>|
|<span data-ttu-id="2bf53-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2bf53-115">Application</span></span>|<span data-ttu-id="2bf53-116">IdentityUserFlow. Read. All, IdentityUserFlow. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2bf53-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bf53-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2bf53-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/userAttributeAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2bf53-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2bf53-118">Optional query parameters</span></span>

<span data-ttu-id="2bf53-119">Este método oferece suporte `$select` `$expand` aos parâmetros e para obter os detalhes do atributo de fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="2bf53-119">This method supports the `$select` and `$expand` parameters to get the details of the user flow attribute.</span></span> <span data-ttu-id="2bf53-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2bf53-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2bf53-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2bf53-121">Request headers</span></span>

|<span data-ttu-id="2bf53-122">Nome</span><span class="sxs-lookup"><span data-stu-id="2bf53-122">Name</span></span>|<span data-ttu-id="2bf53-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bf53-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2bf53-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="2bf53-124">Authorization</span></span>|<span data-ttu-id="2bf53-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2bf53-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bf53-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2bf53-127">Request body</span></span>

<span data-ttu-id="2bf53-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2bf53-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bf53-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bf53-129">Response</span></span>

<span data-ttu-id="2bf53-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2bf53-130">If successful, this method returns a `200 OK` response code and a collection of [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2bf53-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2bf53-131">Examples</span></span>

### <a name="example-1-list-userattributeassignments-in-a-b2cidentityuserflow"></a><span data-ttu-id="2bf53-132">Exemplo 1: list userAttributeAssignments em um b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="2bf53-132">Example 1: List userAttributeAssignments in a b2cIdentityUserFlow</span></span>

#### <a name="request"></a><span data-ttu-id="2bf53-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2bf53-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments?
```

#### <a name="response"></a><span data-ttu-id="2bf53-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bf53-134">Response</span></span>

<span data-ttu-id="2bf53-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2bf53-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-list-userattributeassignments-in-a-b2cidentityuserflow-and-expand-userattribute"></a><span data-ttu-id="2bf53-136">Exemplo 2: list userAttributeAssignments em um b2cIdentityUserFlow e expanda userattribute</span><span class="sxs-lookup"><span data-stu-id="2bf53-136">Example 2: List userAttributeAssignments in a b2cIdentityUserFlow and expand userAttribute</span></span>

#### <a name="request"></a><span data-ttu-id="2bf53-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2bf53-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment_expand"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments?$expand=userAttribute
```

#### <a name="response"></a><span data-ttu-id="2bf53-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bf53-138">Response</span></span>

<span data-ttu-id="2bf53-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2bf53-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
