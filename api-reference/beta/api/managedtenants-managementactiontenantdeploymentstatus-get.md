---
title: Obter managementActionTenantDeploymentStatus
description: Leia as propriedades e as relações de um objeto managementActionTenantDeploymentStatus.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 9efb91eed729ed88d7f95554d752d85e1510480b
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401973"
---
# <a name="get-managementactiontenantdeploymentstatus"></a><span data-ttu-id="c160c-103">Obter managementActionTenantDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="c160c-103">Get managementActionTenantDeploymentStatus</span></span>
<span data-ttu-id="c160c-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="c160c-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c160c-105">Leia as propriedades e as relações de [um objeto managementActionTenantDeploymentStatus.](../resources/managedtenants-managementactiontenantdeploymentstatus.md)</span><span class="sxs-lookup"><span data-stu-id="c160c-105">Read the properties and relationships of a [managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c160c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c160c-106">Permissions</span></span>
<span data-ttu-id="c160c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c160c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c160c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c160c-109">Permission type</span></span>|<span data-ttu-id="c160c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c160c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c160c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c160c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c160c-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c160c-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="c160c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c160c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c160c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c160c-114">Not supported.</span></span>|
|<span data-ttu-id="c160c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c160c-115">Application</span></span>|<span data-ttu-id="c160c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c160c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c160c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c160c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/{managementActionTenantDeploymentStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c160c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c160c-118">Optional query parameters</span></span>
<span data-ttu-id="c160c-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="c160c-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c160c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c160c-120">Request headers</span></span>
|<span data-ttu-id="c160c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c160c-121">Name</span></span>|<span data-ttu-id="c160c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c160c-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="c160c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c160c-123">Authorization</span></span>|<span data-ttu-id="c160c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c160c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c160c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c160c-126">Request body</span></span>
<span data-ttu-id="c160c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c160c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c160c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c160c-128">Response</span></span>

<span data-ttu-id="c160c-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c160c-129">If successful, this method returns a `200 OK` response code and a [managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c160c-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c160c-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c160c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c160c-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_managementactiontenantdeploymentstatus"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/{managementActionTenantDeploymentStatusId}
```

### <a name="response"></a><span data-ttu-id="c160c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c160c-132">Response</span></span>
><span data-ttu-id="c160c-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c160c-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managementActionTenantDeploymentStatus"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/$entity",
    "id": "df7aed9c-c05a-4fc9-b958-64fafaed911d_34298981-4fc8-4974-9486-c8909ed1521b",
    "tenantGroupId": "df7aed9c-c05a-4fc9-b958-64fafaed911d",
    "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
    "statuses": [
        {
            "managementTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
            "managementActionId": "4274db74-99c4-40be-bbeb-da4351136be2",
            "status": "completed",
            "workloadActionDeploymentStatuses": [
                {
                    "actionId": "fcb7ace7-3ea6-4474-912a-00ee78554445",
                    "status": "completed",
                    "deployedPolicyId": "949e8893-68fb-4c9d-b8a0-13c229a7e397",
                    "lastDeploymentDateTime": "2021-06-22T04:09:20.3054223Z",
                    "error": null
                }
            ]
        },
        {
            "managementTemplateId": "31d57d29-2d54-4074-84bd-51c008c2e6b2",
            "managementActionId": "f104bb7f-4854-4209-ba09-c3788f9894c5",
            "status": "completed",
            "workloadActionDeploymentStatuses": [
                {
                    "actionId": "00a9a585-f51c-4b68-b4f5-f0c3165df8ac",
                    "status": "completed",
                    "deployedPolicyId": "19a8d6a6-d87e-4059-85b3-c73bfc5cea15",
                    "lastDeploymentDateTime": "2021-06-22T17:01:44.851214Z",
                    "error": null
                }
            ]
        }
    ]
}
```
