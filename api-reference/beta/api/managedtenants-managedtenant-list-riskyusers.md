---
title: Listar riskyUsers
description: Obter uma lista dos objetos riskyUser e suas propriedades.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 5c1f16969df71d9da8844fca7ff3a905a23a8838
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402123"
---
# <a name="list-riskyusers"></a><span data-ttu-id="1d20f-103">Listar riskyUsers</span><span class="sxs-lookup"><span data-stu-id="1d20f-103">List riskyUsers</span></span>
<span data-ttu-id="1d20f-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="1d20f-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d20f-105">Obter uma lista dos [objetos riskyUser](../resources/managedtenants-riskyuser.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="1d20f-105">Get a list of the [riskyUser](../resources/managedtenants-riskyuser.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d20f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1d20f-106">Permissions</span></span>
<span data-ttu-id="1d20f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d20f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d20f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d20f-109">Permission type</span></span>|<span data-ttu-id="1d20f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1d20f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d20f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d20f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1d20f-112">IdentityRiskyUser.Read.All, IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d20f-112">IdentityRiskyUser.Read.All, IdentityRiskyUser.ReadWrite.All</span></span>|
|<span data-ttu-id="1d20f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d20f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d20f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d20f-114">Not supported.</span></span>|
|<span data-ttu-id="1d20f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1d20f-115">Application</span></span>|<span data-ttu-id="1d20f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d20f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d20f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d20f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/riskyUsers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1d20f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1d20f-118">Optional query parameters</span></span>
<span data-ttu-id="1d20f-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="1d20f-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1d20f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d20f-120">Request headers</span></span>
|<span data-ttu-id="1d20f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="1d20f-121">Name</span></span>|<span data-ttu-id="1d20f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d20f-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1d20f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d20f-123">Authorization</span></span>|<span data-ttu-id="1d20f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d20f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d20f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d20f-126">Request body</span></span>
<span data-ttu-id="1d20f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1d20f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1d20f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d20f-128">Response</span></span>

<span data-ttu-id="1d20f-129">Se tiver êxito, este método retornará um código de resposta e uma coleção de objetos `200 OK` [riskyUser](../resources/managedtenants-riskyuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d20f-129">If successful, this method returns a `200 OK` response code and a collection of [riskyUser](../resources/managedtenants-riskyuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1d20f-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1d20f-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1d20f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d20f-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_riskyuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/riskyUsers
```


### <a name="response"></a><span data-ttu-id="1d20f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d20f-132">Response</span></span>
><span data-ttu-id="1d20f-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1d20f-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.riskyUser)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#riskyUsers",
  "value": [
    {
      "id": "34298981-4fc8-4974-9486-c8909ed1521b_ae8d3a3f-be95-429c-8063-635ccc16e899",
      "userId": "ae8d3a3f-be95-429c-8063-635ccc16e899",
      "userDisplayName": "Cynthia Becker",
      "userPrincipalName": "cynthia@fourthcoffee002.onmicrosoft.com",
      "riskState": "atRisk",
      "riskLevel": "hidden",
      "riskDetail": "hidden",
      "isDeleted": false,
      "riskLastUpdatedDateTime": "2021-06-10T13:58:34.5171907Z",
      "lastRefreshedDateTime": "2021-07-11T11:32:55.2168558Z",
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
      "tenantDisplayName": "Fourth Coffee"
    },
    {
      "id": "38227791-a88b-4fcc-81c5-58cf77668320_05ec33c0-471d-4b1a-901c-093fc65c6401",
      "userId": "05ec33c0-471d-4b1a-901c-093fc65c6401",
      "userDisplayName": "Ina Anthony",
      "userPrincipalName": "ianthony@consolidatedmessenger001.onmicrosoft.com",
      "riskState": "atRisk",
      "riskLevel": "hidden",
      "riskDetail": "hidden",
      "isDeleted": false,
      "riskLastUpdatedDateTime": "2021-06-11T14:35:29.8061797Z",
      "lastRefreshedDateTime": "2021-07-11T14:42:10.8700665Z",
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
      "tenantDisplayName": "Consolidated Messenger"
    }
  ]
}
```
