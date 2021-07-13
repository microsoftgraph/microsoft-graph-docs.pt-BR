---
title: Gerenciamento de listasActions
description: Obter uma lista dos objetos managementAction e suas propriedades.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 03aedec0464908bf25deb004e6cbe4bdb5027acb
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401907"
---
# <a name="list-managementactions"></a><span data-ttu-id="1d9f4-103">Gerenciamento de listasActions</span><span class="sxs-lookup"><span data-stu-id="1d9f4-103">List managementActions</span></span>
<span data-ttu-id="1d9f4-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="1d9f4-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d9f4-105">Obter uma lista dos [objetos managementAction](../resources/managedtenants-managementaction.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-105">Get a list of the [managementAction](../resources/managedtenants-managementaction.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d9f4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d9f4-106">Permissions</span></span>
<span data-ttu-id="1d9f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d9f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d9f4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d9f4-109">Permission type</span></span>|<span data-ttu-id="1d9f4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1d9f4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d9f4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d9f4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1d9f4-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d9f4-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="1d9f4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d9f4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d9f4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-114">Not supported.</span></span>|
|<span data-ttu-id="1d9f4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d9f4-115">Application</span></span>|<span data-ttu-id="1d9f4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d9f4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d9f4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managementActions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1d9f4-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1d9f4-118">Optional query parameters</span></span>
<span data-ttu-id="1d9f4-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="1d9f4-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d9f4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d9f4-120">Request headers</span></span>
|<span data-ttu-id="1d9f4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1d9f4-121">Name</span></span>|<span data-ttu-id="1d9f4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d9f4-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1d9f4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d9f4-123">Authorization</span></span>|<span data-ttu-id="1d9f4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d9f4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d9f4-126">Request body</span></span>
<span data-ttu-id="1d9f4-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d9f4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d9f4-128">Response</span></span>

<span data-ttu-id="1d9f4-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos managementAction](../resources/managedtenants-managementaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-129">If successful, this method returns a `200 OK` response code and a collection of [managementAction](../resources/managedtenants-managementaction.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1d9f4-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1d9f4-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1d9f4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d9f4-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_managementaction"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActions
```


### <a name="response"></a><span data-ttu-id="1d9f4-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d9f4-132">Response</span></span>
><span data-ttu-id="1d9f4-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1d9f4-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.managementAction)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managementActions",
    "value": [
        {
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
    ]
}
```
