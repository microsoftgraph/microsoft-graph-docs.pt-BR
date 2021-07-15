---
title: Gerenciamento de listasTemplates
description: Obter uma lista dos objetos managementTemplate e suas propriedades.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 624e786738efbe2e89052e6321f02b838b7e5c1c
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53443022"
---
# <a name="list-managementtemplates"></a><span data-ttu-id="ce4bb-103">Gerenciamento de listasTemplates</span><span class="sxs-lookup"><span data-stu-id="ce4bb-103">List managementTemplates</span></span>
<span data-ttu-id="ce4bb-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="ce4bb-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce4bb-105">Obter uma lista dos [objetos managementTemplate](../resources/managedtenants-managementtemplate.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="ce4bb-105">Get a list of the [managementTemplate](../resources/managedtenants-managementtemplate.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce4bb-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ce4bb-106">Permissions</span></span>
<span data-ttu-id="ce4bb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce4bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce4bb-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ce4bb-109">Permission type</span></span>|<span data-ttu-id="ce4bb-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ce4bb-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce4bb-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ce4bb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ce4bb-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce4bb-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="ce4bb-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ce4bb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce4bb-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce4bb-114">Not supported.</span></span>|
|<span data-ttu-id="ce4bb-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ce4bb-115">Application</span></span>|<span data-ttu-id="ce4bb-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ce4bb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce4bb-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ce4bb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managementTemplates
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ce4bb-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ce4bb-118">Optional query parameters</span></span>
<span data-ttu-id="ce4bb-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="ce4bb-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce4bb-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ce4bb-120">Request headers</span></span>
|<span data-ttu-id="ce4bb-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ce4bb-121">Name</span></span>|<span data-ttu-id="ce4bb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce4bb-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ce4bb-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ce4bb-123">Authorization</span></span>|<span data-ttu-id="ce4bb-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ce4bb-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce4bb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ce4bb-126">Request body</span></span>
<span data-ttu-id="ce4bb-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ce4bb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce4bb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce4bb-128">Response</span></span>

<span data-ttu-id="ce4bb-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos managementTemplate](../resources/managedtenants-managementtemplate.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ce4bb-129">If successful, this method returns a `200 OK` response code and a collection of [managementTemplate](../resources/managedtenants-managementtemplate.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ce4bb-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ce4bb-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ce4bb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ce4bb-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ce4bb-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce4bb-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_managementtemplate"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementTemplates
```
# <a name="c"></a>[<span data-ttu-id="ce4bb-133">C#</span><span class="sxs-lookup"><span data-stu-id="ce4bb-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-managementtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce4bb-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce4bb-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-managementtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce4bb-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce4bb-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-managementtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ce4bb-136">Java</span><span class="sxs-lookup"><span data-stu-id="ce4bb-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-managementtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ce4bb-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="ce4bb-137">Response</span></span>
><span data-ttu-id="ce4bb-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ce4bb-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.managementTemplate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managementTemplates",
  "value": [
    {
      "id": "e5834405-43d2-4815-867d-3dd600308d1c_1",
      "displayName": "Baseline - Block Legacy Authentication",
      "description": null,
      "category": "identity",
      "parameters": [
        {
          "valueType": "string",
          "displayName": "DisplayName",
          "description": null,
          "jsonDefaultValue": "\"Baseline - Block Legacy Authentication\"",
          "jsonAllowedValues": "null"
        },
        {
          "valueType": "string",
          "displayName": "State",
          "description": null,
          "jsonDefaultValue": "\"enabledForReportingButNotEnforced\"",
          "jsonAllowedValues": "[\"enabled\",\"disabled\",\"enabledForReportingButNotEnforced\"]"
        },
        {
          "valueType": "stringCollection",
          "displayName": "ClientAppTypes",
          "description": null,
          "jsonDefaultValue": "[\"exchangeActiveSync\",\"other\"]",
          "jsonAllowedValues": "[\"exchangeActiveSync\",\"other\"]"
        },
        {
          "valueType": "stringCollection",
          "displayName": "IncludeApplications",
          "description": null,
          "jsonDefaultValue": "[\"All\"]",
          "jsonAllowedValues": "[\"All\"]"
        },
        {
          "valueType": "stringCollection",
          "displayName": "IncludeUsers",
          "description": null,
          "jsonDefaultValue": "[\"None\"]",
          "jsonAllowedValues": "[\"All\",\"None\"]"
        },
        {
          "valueType": "stringCollection",
          "displayName": "IncludeLocations",
          "description": null,
          "jsonDefaultValue": "[\"All\"]",
          "jsonAllowedValues": "[\"All\",\"AllTrusted\"]"
        },
        {
          "valueType": "string",
          "displayName": "GrantControls.Operator",
          "description": null,
          "jsonDefaultValue": "\"OR\"",
          "jsonAllowedValues": "[\"OR\",\"AND\"]"
        },
        {
          "valueType": "stringCollection",
          "displayName": "GrantControls.BuiltInControls",
          "description": null,
          "jsonDefaultValue": "[\"block\"]",
          "jsonAllowedValues": "[\"block\"]"
        }
      ],
      "workloadActions": [
        {
          "actionId": "6a3ad0bc-5d7e-4a49-a105-c559aa4633e1",
          "category": "automated",
          "displayName": "ConditionalAccessPolicy",
          "description": null,
          "service": "AAD",
          "settings": [
            {
              "valueType": "string",
              "displayName": "DisplayName",
              "overwriteAllowed": false,
              "jsonValue": "\"Baseline - Block Legacy Authentication\""
            },
            {
              "valueType": "string",
              "displayName": "State",
              "overwriteAllowed": false,
              "jsonValue": "\"enabledForReportingButNotEnforced\""
            },
            {
              "valueType": "stringCollection",
              "displayName": "ClientAppTypes",
              "overwriteAllowed": false,
              "jsonValue": "[\"exchangeActiveSync\",\"other\"]"
            },
            {
              "valueType": "stringCollection",
              "displayName": "IncludeApplications",
              "overwriteAllowed": false,
              "jsonValue": "[\"All\"]"
            },
            {
              "valueType": "stringCollection",
              "displayName": "IncludeUsers",
              "overwriteAllowed": false,
              "jsonValue": "[\"None\"]"
            },
            {
              "valueType": "stringCollection",
              "displayName": "IncludeLocations",
              "overwriteAllowed": false,
              "jsonValue": "[\"All\"]"
            },
            {
              "valueType": "string",
              "displayName": "GrantControls.Operator",
              "overwriteAllowed": false,
              "jsonValue": "\"OR\""
            },
            {
              "valueType": "stringCollection",
              "displayName": "GrantControls.BuiltInControls",
              "overwriteAllowed": false,
              "jsonValue": "[\"block\"]"
            }
          ]
        }
      ]
    }
  ]
}
```
