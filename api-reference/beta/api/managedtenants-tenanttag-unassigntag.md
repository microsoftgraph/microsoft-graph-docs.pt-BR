---
title: 'tenantTag: unassignTag'
description: Não atribui a marca de locatário dos locatários gerenciados especificados.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: c4cb34b12c075ee44df36baf57cdd14a6739f2d9
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402118"
---
# <a name="tenanttag-unassigntag"></a><span data-ttu-id="a3195-103">tenantTag: unassignTag</span><span class="sxs-lookup"><span data-stu-id="a3195-103">tenantTag: unassignTag</span></span>
<span data-ttu-id="a3195-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="a3195-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3195-105">Não atribui a marca de locatário dos locatários gerenciados especificados.</span><span class="sxs-lookup"><span data-stu-id="a3195-105">Un-assigns the tenant tag from the specified managed tenants.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3195-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="a3195-106">Permissions</span></span>
<span data-ttu-id="a3195-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3195-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3195-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3195-109">Permission type</span></span>|<span data-ttu-id="a3195-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a3195-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3195-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3195-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a3195-112">ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="a3195-112">ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="a3195-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3195-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3195-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3195-114">Not supported.</span></span>|
|<span data-ttu-id="a3195-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3195-115">Application</span></span>|<span data-ttu-id="a3195-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3195-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3195-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3195-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/tenantTags/{tenantTagId}/unassignTag
```

## <a name="request-headers"></a><span data-ttu-id="a3195-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3195-118">Request headers</span></span>
|<span data-ttu-id="a3195-119">Nome</span><span class="sxs-lookup"><span data-stu-id="a3195-119">Name</span></span>|<span data-ttu-id="a3195-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3195-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a3195-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3195-121">Authorization</span></span>|<span data-ttu-id="a3195-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3195-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a3195-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a3195-124">Content-Type</span></span>|<span data-ttu-id="a3195-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3195-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3195-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3195-127">Request body</span></span>
<span data-ttu-id="a3195-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="a3195-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="a3195-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="a3195-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="a3195-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a3195-130">Parameter</span></span>|<span data-ttu-id="a3195-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3195-131">Type</span></span>|<span data-ttu-id="a3195-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3195-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3195-133">tenantIds</span><span class="sxs-lookup"><span data-stu-id="a3195-133">tenantIds</span></span>|<span data-ttu-id="a3195-134">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a3195-134">String collection</span></span>|<span data-ttu-id="a3195-135">A coleção de Azure Active Directory de locatários para locatários gerenciados.</span><span class="sxs-lookup"><span data-stu-id="a3195-135">The collection of Azure Active Directory tenant identifiers for managed tenants.</span></span>|

## <a name="response"></a><span data-ttu-id="a3195-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3195-136">Response</span></span>

<span data-ttu-id="a3195-137">Se tiver êxito, essa ação retornará um código `200 OK` de resposta e um [tenantTag](../resources/managedtenants-tenanttag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3195-137">If successful, this action returns a `200 OK` response code and a [tenantTag](../resources/managedtenants-tenanttag.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a3195-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a3195-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a3195-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3195-139">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "tenanttag_unassigntag"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags/{tenantTagId}/unassignTag
Content-Type: application/json
Content-length: 41

{
  "tenantIds": [
    "String"
  ]
}
```

### <a name="response"></a><span data-ttu-id="a3195-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3195-140">Response</span></span>
><span data-ttu-id="a3195-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a3195-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantTag"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantTags/$entity",
  "id": "2a66c69f-87ec-4fb3-a797-dd500cc3454d",
  "displayName": "Support",
  "description": "Tenants that has purcahsed support",
  "tenants": [],
  "isDeleted": null,
  "createdDateTime": "2021-06-26T13:51:23.3927236Z",
  "createdByUserId": "65ca7649-4ccb-4823-9c39-42bd75191bf8",
  "lastActionDateTime": "2021-07-11T19:57:56.4242898Z",
  "lastActionByUserId": "50bf7bd8-1b3a-4d1d-94c5-86d27e68857f"
}
```
