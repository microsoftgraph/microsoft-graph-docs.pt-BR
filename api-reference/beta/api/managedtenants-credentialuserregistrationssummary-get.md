---
title: Obter credentialUserRegistrationsSummary
description: Leia as propriedades e as relações de um objeto credentialUserRegistrationsSummary.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 96e74fa01a0e3b76dd268596e33aed981abc3563
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401925"
---
# <a name="get-credentialuserregistrationssummary"></a><span data-ttu-id="690c7-103">Obter credentialUserRegistrationsSummary</span><span class="sxs-lookup"><span data-stu-id="690c7-103">Get credentialUserRegistrationsSummary</span></span>
<span data-ttu-id="690c7-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="690c7-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="690c7-105">Leia as propriedades e as relações de [um objeto credentialUserRegistrationsSummary.](../resources/managedtenants-credentialuserregistrationssummary.md)</span><span class="sxs-lookup"><span data-stu-id="690c7-105">Read the properties and relationships of a [credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="690c7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="690c7-106">Permissions</span></span>
<span data-ttu-id="690c7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="690c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="690c7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="690c7-109">Permission type</span></span>|<span data-ttu-id="690c7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="690c7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="690c7-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="690c7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="690c7-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="690c7-112">Reports.Read.All</span></span>|
|<span data-ttu-id="690c7-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="690c7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="690c7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="690c7-114">Not supported.</span></span>|
|<span data-ttu-id="690c7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="690c7-115">Application</span></span>|<span data-ttu-id="690c7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="690c7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="690c7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="690c7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/credentialUserRegistrationsSummaries/{credentialUserRegistrationsSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="690c7-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="690c7-118">Optional query parameters</span></span>
<span data-ttu-id="690c7-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="690c7-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="690c7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="690c7-120">Request headers</span></span>
|<span data-ttu-id="690c7-121">Nome</span><span class="sxs-lookup"><span data-stu-id="690c7-121">Name</span></span>|<span data-ttu-id="690c7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="690c7-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="690c7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="690c7-123">Authorization</span></span>|<span data-ttu-id="690c7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="690c7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="690c7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="690c7-126">Request body</span></span>
<span data-ttu-id="690c7-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="690c7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="690c7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="690c7-128">Response</span></span>

<span data-ttu-id="690c7-129">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="690c7-129">If successful, this method returns a `200 OK` response code and a [credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="690c7-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="690c7-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="690c7-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="690c7-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_credentialuserregistrationssummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/credentialUserRegistrationsSummaries/{credentialUserRegistrationsSummaryId}
```

### <a name="response"></a><span data-ttu-id="690c7-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="690c7-132">Response</span></span>
><span data-ttu-id="690c7-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="690c7-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.credentialUserRegistrationsSummary"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.credentialUserRegistrationsSummary",
    "id": "34298981-4fc8-4974-9486-c8909ed1521b",
    "mfaAndSsprCapableUserCount": 0,
    "ssprEnabledUserCount": 1,
    "mfaRegisteredUserCount": 0,
    "ssprRegisteredUserCount": 0,
    "totalUserCount": 7,
    "securityDefaultsEnabled": false,
    "mfaConditionalAccessPolicyState": "enabledForReportingButNotEnforced",
    "lastRefreshedDateTime": "2021-07-11T11:15:52.9375367Z",
    "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
    "tenantDisplayName": "Fourth Coffee"
}
```
