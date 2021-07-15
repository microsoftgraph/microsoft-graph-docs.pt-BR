---
title: 'tenantTag: assignTag'
description: Atribua a marca de locatário aos locatários gerenciados especificados.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 867f252eca5fc84f5f77e916c38d50bd564b7e9a
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441742"
---
# <a name="tenanttag-assigntag"></a><span data-ttu-id="2a932-103">tenantTag: assignTag</span><span class="sxs-lookup"><span data-stu-id="2a932-103">tenantTag: assignTag</span></span>
<span data-ttu-id="2a932-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="2a932-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a932-105">Atribua a marca de locatário aos locatários gerenciados especificados.</span><span class="sxs-lookup"><span data-stu-id="2a932-105">Assign the tenant tag to the specified managed tenants.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a932-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="2a932-106">Permissions</span></span>
<span data-ttu-id="2a932-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a932-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a932-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a932-109">Permission type</span></span>|<span data-ttu-id="2a932-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2a932-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a932-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a932-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2a932-112">ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="2a932-112">ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="2a932-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a932-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a932-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a932-114">Not supported.</span></span>|
|<span data-ttu-id="2a932-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a932-115">Application</span></span>|<span data-ttu-id="2a932-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a932-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a932-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a932-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /tenantRelationships/managedTenants/tenantTags/{tenantTagId}/assignTag
```

## <a name="request-headers"></a><span data-ttu-id="2a932-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a932-118">Request headers</span></span>
|<span data-ttu-id="2a932-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2a932-119">Name</span></span>|<span data-ttu-id="2a932-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a932-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2a932-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a932-121">Authorization</span></span>|<span data-ttu-id="2a932-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a932-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2a932-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2a932-124">Content-Type</span></span>|<span data-ttu-id="2a932-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a932-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a932-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a932-127">Request body</span></span>
<span data-ttu-id="2a932-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="2a932-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2a932-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="2a932-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2a932-130">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2a932-130">Parameter</span></span>|<span data-ttu-id="2a932-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a932-131">Type</span></span>|<span data-ttu-id="2a932-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a932-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a932-133">tenantIds</span><span class="sxs-lookup"><span data-stu-id="2a932-133">tenantIds</span></span>|<span data-ttu-id="2a932-134">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="2a932-134">String collection</span></span>|<span data-ttu-id="2a932-135">A coleção de Azure Active Directory de locatários onde a marca de locatário deve ser atribuída.</span><span class="sxs-lookup"><span data-stu-id="2a932-135">The collection of Azure Active Directory tenant identifiers where the tenant tag should be assigned.</span></span>|

## <a name="response"></a><span data-ttu-id="2a932-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a932-136">Response</span></span>

<span data-ttu-id="2a932-137">Se tiver êxito, essa ação retornará um código `200 OK` de resposta e um [tenantTag](../resources/managedtenants-tenanttag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a932-137">If successful, this action returns a `200 OK` response code and a [tenantTag](../resources/managedtenants-tenanttag.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2a932-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2a932-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2a932-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a932-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2a932-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a932-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "tenanttag_assigntag"
}
-->
``` http
POST https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags/{tenantTagId}/assignTag
Content-Type: application/json
Content-length: 41

{
  "tenantIds": [
    "String"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="2a932-141">C#</span><span class="sxs-lookup"><span data-stu-id="2a932-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/tenanttag-assigntag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a932-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a932-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/tenanttag-assigntag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a932-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a932-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/tenanttag-assigntag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2a932-144">Java</span><span class="sxs-lookup"><span data-stu-id="2a932-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/tenanttag-assigntag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2a932-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a932-145">Response</span></span>
><span data-ttu-id="2a932-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="2a932-146">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "id": "34298981-4fc8-4974-9486-c8909ed1521b",
  "displayName": "Support",
  "description": "Tenants that have purchased support",
  "tenants": [
    {
      "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b"
    }
  ],
  "isDeleted": null,
  "createdDateTime": "2021-06-26T13:51:23.3927236Z",
  "createdByUserId": "65ca7649-4ccb-4823-9c39-42bd75191bf8",
  "lastActionDateTime": "2021-07-11T19:55:19.7230386Z",
  "lastActionByUserId": "50bf7bd8-1b3a-4d1d-94c5-86d27e68857f"
}
```
