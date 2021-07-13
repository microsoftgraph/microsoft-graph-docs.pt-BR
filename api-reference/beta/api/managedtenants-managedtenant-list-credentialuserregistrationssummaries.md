---
title: Listar credentialUserRegistrationsSummaries
description: Obter uma lista dos objetos credentialUserRegistrationsSummary e suas propriedades.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: fcb42f7c00a518e270d4e937156e1e6f39b4b692
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401908"
---
# <a name="list-credentialuserregistrationssummaries"></a><span data-ttu-id="47a1c-103">Listar credentialUserRegistrationsSummaries</span><span class="sxs-lookup"><span data-stu-id="47a1c-103">List credentialUserRegistrationsSummaries</span></span>
<span data-ttu-id="47a1c-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="47a1c-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47a1c-105">Obter uma lista dos [objetos credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="47a1c-105">Get a list of the [credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="47a1c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="47a1c-106">Permissions</span></span>
<span data-ttu-id="47a1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47a1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47a1c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="47a1c-109">Permission type</span></span>|<span data-ttu-id="47a1c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="47a1c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47a1c-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="47a1c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="47a1c-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="47a1c-112">Reports.Read.All</span></span>|
|<span data-ttu-id="47a1c-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="47a1c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47a1c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47a1c-114">Not supported.</span></span>|
|<span data-ttu-id="47a1c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="47a1c-115">Application</span></span>|<span data-ttu-id="47a1c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="47a1c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47a1c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="47a1c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/credentialUserRegistrationsSummaries
```

## <a name="optional-query-parameters"></a><span data-ttu-id="47a1c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="47a1c-118">Optional query parameters</span></span>
<span data-ttu-id="47a1c-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="47a1c-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="47a1c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="47a1c-120">Request headers</span></span>
|<span data-ttu-id="47a1c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="47a1c-121">Name</span></span>|<span data-ttu-id="47a1c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="47a1c-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="47a1c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="47a1c-123">Authorization</span></span>|<span data-ttu-id="47a1c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="47a1c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="47a1c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="47a1c-126">Request body</span></span>
<span data-ttu-id="47a1c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="47a1c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47a1c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="47a1c-128">Response</span></span>

<span data-ttu-id="47a1c-129">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="47a1c-129">If successful, this method returns a `200 OK` response code and a collection of [credentialUserRegistrationsSummary](../resources/managedtenants-credentialuserregistrationssummary.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="47a1c-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="47a1c-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="47a1c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="47a1c-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_credentialuserregistrationssummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/credentialUserRegistrationsSummaries
```


### <a name="response"></a><span data-ttu-id="47a1c-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="47a1c-132">Response</span></span>
><span data-ttu-id="47a1c-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="47a1c-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.credentialUserRegistrationsSummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#credentialUserRegistrationsSummaries",
  "value": [
    {
      "id": "38227791-a88b-4fcc-81c5-58cf77668320",
      "mfaAndSsprCapableUserCount": 2,
      "ssprEnabledUserCount": 9,
      "mfaRegisteredUserCount": 3,
      "ssprRegisteredUserCount": 2,
      "totalUserCount": 9,
      "securityDefaultsEnabled": false,
      "mfaConditionalAccessPolicyState": "enabled",
      "lastRefreshedDateTime": "2021-07-11T09:58:11.5730661Z",
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
      "tenantDisplayName": "Consolidated Messenger"
    },
    {
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
  ]
}
```
