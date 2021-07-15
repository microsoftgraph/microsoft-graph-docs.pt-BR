---
title: Obter tenantTag
description: Leia as propriedades e as relações de um objeto tenantTag.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 711adc2987df3b2707ea8a23e8a06c45f4cb398d
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441055"
---
# <a name="get-tenanttag"></a><span data-ttu-id="730d4-103">Obter tenantTag</span><span class="sxs-lookup"><span data-stu-id="730d4-103">Get tenantTag</span></span>
<span data-ttu-id="730d4-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="730d4-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="730d4-105">Leia as propriedades e as relações de um [objeto tenantTag.](../resources/managedtenants-tenanttag.md)</span><span class="sxs-lookup"><span data-stu-id="730d4-105">Read the properties and relationships of a [tenantTag](../resources/managedtenants-tenanttag.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="730d4-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="730d4-106">Permissions</span></span>
<span data-ttu-id="730d4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="730d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="730d4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="730d4-109">Permission type</span></span>|<span data-ttu-id="730d4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="730d4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="730d4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="730d4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="730d4-112">ManagedTenants.Read.All, ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="730d4-112">ManagedTenants.Read.All, ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="730d4-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="730d4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="730d4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="730d4-114">Not supported.</span></span>|
|<span data-ttu-id="730d4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="730d4-115">Application</span></span>|<span data-ttu-id="730d4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="730d4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="730d4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="730d4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenantTags/{tenantTagId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="730d4-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="730d4-118">Optional query parameters</span></span>
<span data-ttu-id="730d4-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$count` , , , , , e `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="730d4-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="730d4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="730d4-120">Request headers</span></span>
|<span data-ttu-id="730d4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="730d4-121">Name</span></span>|<span data-ttu-id="730d4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="730d4-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="730d4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="730d4-123">Authorization</span></span>|<span data-ttu-id="730d4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="730d4-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="730d4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="730d4-126">Request body</span></span>
<span data-ttu-id="730d4-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="730d4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="730d4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="730d4-128">Response</span></span>

<span data-ttu-id="730d4-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [tenantTag](../resources/managedtenants-tenanttag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="730d4-129">If successful, this method returns a `200 OK` response code and a [tenantTag](../resources/managedtenants-tenanttag.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="730d4-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="730d4-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="730d4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="730d4-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="730d4-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="730d4-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_tenanttag"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags/{tenantTagId}
```
# <a name="c"></a>[<span data-ttu-id="730d4-133">C#</span><span class="sxs-lookup"><span data-stu-id="730d4-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-tenanttag-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="730d4-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="730d4-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-tenanttag-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="730d4-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="730d4-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-tenanttag-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="730d4-136">Java</span><span class="sxs-lookup"><span data-stu-id="730d4-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-tenanttag-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="730d4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="730d4-137">Response</span></span>
><span data-ttu-id="730d4-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="730d4-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/tenantTags/$entity",
    "id": "913391c0-5466-42b4-900d-0a7501399cb0",
    "displayName": "Onboarding",
    "description": "Tenants that we are currently onboarding",
    "tenantIds": [
        "38227791-a88b-4fcc-81c5-58cf77668320",
        "34298981-4fc8-4974-9486-c8909ed1521b",
        "4d262a25-c70a-430b-9e8e-46c31dec116b"
    ],
    "isDeleted": null,
    "createdDateTime": "2021-06-16T20:36:31.086644Z",
    "createdByUserId": "9bf6a5ad-aecb-4194-a16b-38e02702a602",
    "lastActionDateTime": "2021-06-28T20:46:09.0071888Z",
    "lastActionByUserId": "08ea0285-30cb-46cc-abc8-3d8422e21ecb",
    "tenants": [
        {
            "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320"
        },
        {
            "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b"
        },
        {
            "tenantId": "4d262a25-c70a-430b-9e8e-46c31dec116b"
        }
    ]
}
```
