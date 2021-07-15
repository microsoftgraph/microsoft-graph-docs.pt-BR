---
title: Obter managementActionTenantDeploymentStatus
description: Leia as propriedades e as relações de um objeto managementActionTenantDeploymentStatus.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: ac7da25234fd72abf979a7c8304a3a53d3554661
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442597"
---
# <a name="get-managementactiontenantdeploymentstatus"></a><span data-ttu-id="8047b-103">Obter managementActionTenantDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="8047b-103">Get managementActionTenantDeploymentStatus</span></span>
<span data-ttu-id="8047b-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="8047b-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8047b-105">Leia as propriedades e as relações de [um objeto managementActionTenantDeploymentStatus.](../resources/managedtenants-managementactiontenantdeploymentstatus.md)</span><span class="sxs-lookup"><span data-stu-id="8047b-105">Read the properties and relationships of a [managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8047b-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="8047b-106">Permissions</span></span>
<span data-ttu-id="8047b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8047b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8047b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8047b-109">Permission type</span></span>|<span data-ttu-id="8047b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8047b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8047b-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8047b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8047b-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8047b-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="8047b-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8047b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8047b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8047b-114">Not supported.</span></span>|
|<span data-ttu-id="8047b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8047b-115">Application</span></span>|<span data-ttu-id="8047b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8047b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8047b-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8047b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/{managementActionTenantDeploymentStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8047b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8047b-118">Optional query parameters</span></span>
<span data-ttu-id="8047b-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="8047b-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8047b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8047b-120">Request headers</span></span>
|<span data-ttu-id="8047b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8047b-121">Name</span></span>|<span data-ttu-id="8047b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8047b-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8047b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8047b-123">Authorization</span></span>|<span data-ttu-id="8047b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8047b-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8047b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8047b-126">Request body</span></span>
<span data-ttu-id="8047b-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8047b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8047b-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8047b-128">Response</span></span>

<span data-ttu-id="8047b-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8047b-129">If successful, this method returns a `200 OK` response code and a [managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8047b-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8047b-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8047b-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8047b-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="8047b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8047b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_managementactiontenantdeploymentstatus"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/{managementActionTenantDeploymentStatusId}
```
# <a name="c"></a>[<span data-ttu-id="8047b-133">C#</span><span class="sxs-lookup"><span data-stu-id="8047b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-managementactiontenantdeploymentstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8047b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8047b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-managementactiontenantdeploymentstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8047b-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8047b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-managementactiontenantdeploymentstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8047b-136">Java</span><span class="sxs-lookup"><span data-stu-id="8047b-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-managementactiontenantdeploymentstatus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8047b-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="8047b-137">Response</span></span>
><span data-ttu-id="8047b-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8047b-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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
