---
title: Obter managementAction
description: Leia as propriedades e as relações de um objeto managementAction.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 46da15bc9101890f9f05e24086dd74dc3c022e0e
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402015"
---
# <a name="get-managementaction"></a><span data-ttu-id="5c5ef-103">Obter managementAction</span><span class="sxs-lookup"><span data-stu-id="5c5ef-103">Get managementAction</span></span>
<span data-ttu-id="5c5ef-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="5c5ef-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c5ef-105">Leia as propriedades e as relações de um [objeto managementAction.](../resources/managedtenants-managementaction.md)</span><span class="sxs-lookup"><span data-stu-id="5c5ef-105">Read the properties and relationships of a [managementAction](../resources/managedtenants-managementaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c5ef-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5c5ef-106">Permissions</span></span>
<span data-ttu-id="5c5ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5c5ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c5ef-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5c5ef-109">Permission type</span></span>|<span data-ttu-id="5c5ef-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5c5ef-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c5ef-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5c5ef-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5c5ef-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c5ef-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="5c5ef-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5c5ef-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c5ef-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c5ef-114">Not supported.</span></span>|
|<span data-ttu-id="5c5ef-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5c5ef-115">Application</span></span>|<span data-ttu-id="5c5ef-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5c5ef-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c5ef-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5c5ef-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managementActions/{managementActionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5c5ef-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5c5ef-118">Optional query parameters</span></span>
<span data-ttu-id="5c5ef-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="5c5ef-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c5ef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c5ef-120">Request headers</span></span>
|<span data-ttu-id="5c5ef-121">Nome</span><span class="sxs-lookup"><span data-stu-id="5c5ef-121">Name</span></span>|<span data-ttu-id="5c5ef-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c5ef-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5c5ef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5c5ef-123">Authorization</span></span>|<span data-ttu-id="5c5ef-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c5ef-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c5ef-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5c5ef-126">Request body</span></span>
<span data-ttu-id="5c5ef-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5c5ef-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c5ef-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c5ef-128">Response</span></span>

<span data-ttu-id="5c5ef-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [managementAction](../resources/managedtenants-managementaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5c5ef-129">If successful, this method returns a `200 OK` response code and a [managementAction](../resources/managedtenants-managementaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5c5ef-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5c5ef-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5c5ef-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5c5ef-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_managementaction"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActions/{managementActionId}
```


### <a name="response"></a><span data-ttu-id="5c5ef-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="5c5ef-132">Response</span></span>
><span data-ttu-id="5c5ef-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5c5ef-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managementAction"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managementActions/$entity",
    "id": "4274db74-99c4-40be-bbeb-da4351136be2",
    "referenceTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
    "displayName": "Baseline - Require MFA for end users",
    "description": null,
    "category": "identity",
    "workloadActions": [
        {
            "actionId": "fcb7ace7-3ea6-4474-912a-00ee78554445",
            "category": "automated",
            "displayName": "ConditionalAccessPolicy",
            "description": null,
            "service": "AAD",
            "settings": [
                {
                    "valueType": "string",
                    "displayName": "DisplayName",
                    "overwriteAllowed": false,
                    "jsonValue": "\"Baseline - Require MFA for end users\""
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
                    "jsonValue": "[\"All\"]"
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
                    "jsonValue": "[\"mfa\"]"
                }
            ]
        }
    ]
}
```
