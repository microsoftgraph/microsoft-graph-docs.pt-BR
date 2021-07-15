---
title: 'tenantTag: unassignTag'
description: Não atribui a marca de locatário dos locatários gerenciados especificados.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 41a2cc35ea47374ef16131fd6190476bcac77847
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442764"
---
# <a name="tenanttag-unassigntag"></a><span data-ttu-id="b99b7-103">tenantTag: unassignTag</span><span class="sxs-lookup"><span data-stu-id="b99b7-103">tenantTag: unassignTag</span></span>
<span data-ttu-id="b99b7-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="b99b7-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b99b7-105">Não atribui a marca de locatário dos locatários gerenciados especificados.</span><span class="sxs-lookup"><span data-stu-id="b99b7-105">Un-assigns the tenant tag from the specified managed tenants.</span></span>

## <a name="permissions"></a><span data-ttu-id="b99b7-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b99b7-106">Permissions</span></span>
<span data-ttu-id="b99b7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b99b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b99b7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b99b7-109">Permission type</span></span>|<span data-ttu-id="b99b7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b99b7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b99b7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b99b7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b99b7-112">ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="b99b7-112">ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="b99b7-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b99b7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b99b7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b99b7-114">Not supported.</span></span>|
|<span data-ttu-id="b99b7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b99b7-115">Application</span></span>|<span data-ttu-id="b99b7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b99b7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b99b7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b99b7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/tenantTags/{tenantTagId}/unassignTag
```

## <a name="request-headers"></a><span data-ttu-id="b99b7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b99b7-118">Request headers</span></span>
|<span data-ttu-id="b99b7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="b99b7-119">Name</span></span>|<span data-ttu-id="b99b7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="b99b7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b99b7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="b99b7-121">Authorization</span></span>|<span data-ttu-id="b99b7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b99b7-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b99b7-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b99b7-124">Content-Type</span></span>|<span data-ttu-id="b99b7-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b99b7-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b99b7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b99b7-127">Request body</span></span>
<span data-ttu-id="b99b7-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b99b7-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b99b7-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="b99b7-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b99b7-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b99b7-130">Parameter</span></span>|<span data-ttu-id="b99b7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b99b7-131">Type</span></span>|<span data-ttu-id="b99b7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b99b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b99b7-133">tenantIds</span><span class="sxs-lookup"><span data-stu-id="b99b7-133">tenantIds</span></span>|<span data-ttu-id="b99b7-134">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b99b7-134">String collection</span></span>|<span data-ttu-id="b99b7-135">A coleção de Azure Active Directory de locatários para locatários gerenciados.</span><span class="sxs-lookup"><span data-stu-id="b99b7-135">The collection of Azure Active Directory tenant identifiers for managed tenants.</span></span>|

## <a name="response"></a><span data-ttu-id="b99b7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="b99b7-136">Response</span></span>

<span data-ttu-id="b99b7-137">Se tiver êxito, essa ação retornará um código `200 OK` de resposta e um [tenantTag](../resources/managedtenants-tenanttag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b99b7-137">If successful, this action returns a `200 OK` response code and a [tenantTag](../resources/managedtenants-tenanttag.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b99b7-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b99b7-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b99b7-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b99b7-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b99b7-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="b99b7-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b99b7-141">C#</span><span class="sxs-lookup"><span data-stu-id="b99b7-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tenanttag-unassigntag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b99b7-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b99b7-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tenanttag-unassigntag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b99b7-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b99b7-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tenanttag-unassigntag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b99b7-144">Java</span><span class="sxs-lookup"><span data-stu-id="b99b7-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tenanttag-unassigntag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b99b7-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="b99b7-145">Response</span></span>
><span data-ttu-id="b99b7-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b99b7-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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
