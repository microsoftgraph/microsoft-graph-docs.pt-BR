---
title: Obter riskyUser
description: Leia as propriedades e as relações de um objeto riskyUser.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 523e5c3abe471ac2951615411c232517895dce64
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441385"
---
# <a name="get-riskyuser"></a><span data-ttu-id="7cc17-103">Obter riskyUser</span><span class="sxs-lookup"><span data-stu-id="7cc17-103">Get riskyUser</span></span>
<span data-ttu-id="7cc17-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="7cc17-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7cc17-105">Leia as propriedades e as relações de um [objeto riskyUser.](../resources/managedtenants-riskyuser.md)</span><span class="sxs-lookup"><span data-stu-id="7cc17-105">Read the properties and relationships of a [riskyUser](../resources/managedtenants-riskyuser.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7cc17-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="7cc17-106">Permissions</span></span>
<span data-ttu-id="7cc17-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cc17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cc17-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7cc17-109">Permission type</span></span>|<span data-ttu-id="7cc17-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7cc17-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cc17-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7cc17-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7cc17-112">IdentityRiskyUser.Read.All, IdentityRiskyUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cc17-112">IdentityRiskyUser.Read.All, IdentityRiskyUser.ReadWrite.All</span></span>|
|<span data-ttu-id="7cc17-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7cc17-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cc17-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7cc17-114">Not supported.</span></span>|
|<span data-ttu-id="7cc17-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7cc17-115">Application</span></span>|<span data-ttu-id="7cc17-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7cc17-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cc17-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7cc17-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/riskyUsers/{riskyUserId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7cc17-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7cc17-118">Optional query parameters</span></span>
<span data-ttu-id="7cc17-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="7cc17-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7cc17-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7cc17-120">Request headers</span></span>
|<span data-ttu-id="7cc17-121">Nome</span><span class="sxs-lookup"><span data-stu-id="7cc17-121">Name</span></span>|<span data-ttu-id="7cc17-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="7cc17-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7cc17-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7cc17-123">Authorization</span></span>|<span data-ttu-id="7cc17-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7cc17-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cc17-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7cc17-126">Request body</span></span>
<span data-ttu-id="7cc17-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7cc17-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7cc17-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cc17-128">Response</span></span>

<span data-ttu-id="7cc17-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [riskyUser](../resources/managedtenants-riskyuser.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7cc17-129">If successful, this method returns a `200 OK` response code and a [riskyUser](../resources/managedtenants-riskyuser.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7cc17-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7cc17-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7cc17-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7cc17-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7cc17-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7cc17-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_riskyuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/riskyUsers/{riskyUserId}
```
# <a name="c"></a>[<span data-ttu-id="7cc17-133">C#</span><span class="sxs-lookup"><span data-stu-id="7cc17-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-riskyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7cc17-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7cc17-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-riskyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7cc17-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7cc17-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-riskyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7cc17-136">Java</span><span class="sxs-lookup"><span data-stu-id="7cc17-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-riskyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="7cc17-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cc17-137">Response</span></span>
><span data-ttu-id="7cc17-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="7cc17-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.riskyUser"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.riskyUser",
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
}
```
