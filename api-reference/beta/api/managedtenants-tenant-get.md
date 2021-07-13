---
title: Obter locatário
description: Leia as propriedades e as relações de um objeto tenant.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: edcf0a8d13ed02245140af4beadf4a472719f1d7
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401975"
---
# <a name="get-tenant"></a><span data-ttu-id="0392e-103">Obter locatário</span><span class="sxs-lookup"><span data-stu-id="0392e-103">Get tenant</span></span>
<span data-ttu-id="0392e-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="0392e-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0392e-105">Leia as propriedades e as relações de um [objeto tenant.](../resources/managedtenants-tenant.md)</span><span class="sxs-lookup"><span data-stu-id="0392e-105">Read the properties and relationships of a [tenant](../resources/managedtenants-tenant.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0392e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0392e-106">Permissions</span></span>
<span data-ttu-id="0392e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0392e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0392e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0392e-109">Permission type</span></span>|<span data-ttu-id="0392e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0392e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0392e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0392e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0392e-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0392e-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="0392e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0392e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0392e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0392e-114">Not supported.</span></span>|
|<span data-ttu-id="0392e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0392e-115">Application</span></span>|<span data-ttu-id="0392e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0392e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0392e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0392e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenants/{tenantId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0392e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0392e-118">Optional query parameters</span></span>
<span data-ttu-id="0392e-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="0392e-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0392e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0392e-120">Request headers</span></span>
|<span data-ttu-id="0392e-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0392e-121">Name</span></span>|<span data-ttu-id="0392e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0392e-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0392e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0392e-123">Authorization</span></span>|<span data-ttu-id="0392e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0392e-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0392e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0392e-126">Request body</span></span>
<span data-ttu-id="0392e-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0392e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0392e-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0392e-128">Response</span></span>

<span data-ttu-id="0392e-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [tenant](../resources/managedtenants-tenant.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0392e-129">If successful, this method returns a `200 OK` response code and a [tenant](../resources/managedtenants-tenant.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0392e-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0392e-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0392e-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0392e-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tenant"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenants/{tenantId}
```


### <a name="response"></a><span data-ttu-id="0392e-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0392e-132">Response</span></span>
><span data-ttu-id="0392e-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0392e-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenant"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.tenant",
  "id": "34298981-4fc8-4974-9486-c8909ed1521b",
  "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
  "contract": {
    "displayName": "Fourth Coffee",
    "defaultDomainName": "fourthcoffe001.onmicrosoft.com",
    "contractType": 2
  },
  "tenantStatusInformation": {
    "onboardingStatus": "ineligible",
    "onboardingDateTime": "2012-02-20T00:00:00Z",
    "onboardedByUserId": "",
    "offboardedDateTime": "2012-02-20T00:00:00Z",
    "offboardedBy": "",
    "delegatedPrivilegeStatus": "delegatedAdminPrivileges",
    "workloadStatuses": [
      {
        "displayName": "Device Management",
        "onboardingStatus": "onboarded",
        "onboardedDateTime": "2012-02-20T00:00:00Z",
        "offboardedDateTime": null
      },
      {
        "displayName": "Cloud PC",
        "onboardingStatus": "notOnboarded",
        "onboardedDateTime": "2012-02-20T00:00:00Z",
        "offboardedDateTime": null
      }
    ]
  },
  "createdDateTime": "2012-02-20T00:00:00Z",
  "lastUpdatedDatetime": "2021-02-20T00:00:00Z"
}
```
