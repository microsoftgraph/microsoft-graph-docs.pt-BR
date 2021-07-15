---
title: Obter managementIntent
description: Leia as propriedades e as relações de um objeto managementIntent.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: f074678ca774e66c659465fe4f7fc37fedd25cd0
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442568"
---
# <a name="get-managementintent"></a><span data-ttu-id="12fee-103">Obter managementIntent</span><span class="sxs-lookup"><span data-stu-id="12fee-103">Get managementIntent</span></span>
<span data-ttu-id="12fee-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="12fee-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12fee-105">Leia as propriedades e as relações de um [objeto managementIntent.](../resources/managedtenants-managementintent.md)</span><span class="sxs-lookup"><span data-stu-id="12fee-105">Read the properties and relationships of a [managementIntent](../resources/managedtenants-managementintent.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="12fee-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="12fee-106">Permissions</span></span>
<span data-ttu-id="12fee-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12fee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12fee-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12fee-109">Permission type</span></span>|<span data-ttu-id="12fee-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="12fee-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12fee-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12fee-111">Delegated (work or school account)</span></span>|<span data-ttu-id="12fee-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12fee-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="12fee-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12fee-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12fee-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12fee-114">Not supported.</span></span>|
|<span data-ttu-id="12fee-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12fee-115">Application</span></span>|<span data-ttu-id="12fee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12fee-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12fee-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12fee-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managementIntents/{managementIntentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="12fee-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="12fee-118">Optional query parameters</span></span>
<span data-ttu-id="12fee-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="12fee-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="12fee-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12fee-120">Request headers</span></span>
|<span data-ttu-id="12fee-121">Nome</span><span class="sxs-lookup"><span data-stu-id="12fee-121">Name</span></span>|<span data-ttu-id="12fee-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="12fee-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="12fee-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="12fee-123">Authorization</span></span>|<span data-ttu-id="12fee-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12fee-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="12fee-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12fee-126">Request body</span></span>
<span data-ttu-id="12fee-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="12fee-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12fee-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="12fee-128">Response</span></span>

<span data-ttu-id="12fee-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [managementIntent](../resources/managedtenants-managementintent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12fee-129">If successful, this method returns a `200 OK` response code and a [managementIntent](../resources/managedtenants-managementintent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="12fee-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="12fee-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="12fee-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12fee-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="12fee-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="12fee-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_managementintent"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementIntents/{managementIntentId}
```
# <a name="c"></a>[<span data-ttu-id="12fee-133">C#</span><span class="sxs-lookup"><span data-stu-id="12fee-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-managementintent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12fee-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12fee-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-managementintent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12fee-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12fee-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-managementintent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="12fee-136">Java</span><span class="sxs-lookup"><span data-stu-id="12fee-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-managementintent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="12fee-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="12fee-137">Response</span></span>
><span data-ttu-id="12fee-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="12fee-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managementIntent"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managementIntents/$entity",
    "id": "586895ab-8a59-4b79-be25-b06949a819bb",
    "displayName": "Default Baseline",
    "isGlobal": true,
    "managementTemplates": [
        {
            "managementTemplateId": "e5834405-43d2-4815-867d-3dd600308d1c",
            "displayName": "Baseline - Block Legacy Authentication",
            "category": "identity"
        },
        {
            "managementTemplateId": "12524106-036f-457f-b7a6-b003509d29c8",
            "displayName": "Baseline - Require MFA for Admins",
            "category": "identity"
        },
        {
            "managementTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
            "displayName": "Baseline - Require MFA for end users",
            "category": "identity"
        },
        {
            "managementTemplateId": "e2cadc41-a08f-45e7-8eb1-942d224dfb9a",
            "displayName": "Baseline - Enroll devices in MEM",
            "category": "devices"
        },
        {
            "managementTemplateId": "31d57d29-2d54-4074-84bd-51c008c2e6b2",
            "displayName": "Baseline - Setup Compliance Policy for Windows 10 devices",
            "category": "devices"
        },
        {
            "managementTemplateId": "b2d6d189-ea31-4cf8-b75e-41210c583127",
            "displayName": "Baseline - Setup Microsoft Defender Antivirus Policy for Windows 10 devices",
            "category": "devices"
        }
    ]
}
```
