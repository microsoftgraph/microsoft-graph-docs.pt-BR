---
title: Listar tenantGroups
description: Obter uma lista dos objetos tenantGroup e suas propriedades.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: c60e656951890cbe6319b1949926a14a5437fe92
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440476"
---
# <a name="list-tenantgroups"></a><span data-ttu-id="dcf89-103">Listar tenantGroups</span><span class="sxs-lookup"><span data-stu-id="dcf89-103">List tenantGroups</span></span>
<span data-ttu-id="dcf89-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="dcf89-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcf89-105">Obter uma lista dos objetos [tenantGroup](../resources/managedtenants-tenantgroup.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="dcf89-105">Get a list of the [tenantGroup](../resources/managedtenants-tenantgroup.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="dcf89-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="dcf89-106">Permissions</span></span>
<span data-ttu-id="dcf89-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dcf89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcf89-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dcf89-109">Permission type</span></span>|<span data-ttu-id="dcf89-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dcf89-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dcf89-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dcf89-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dcf89-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcf89-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="dcf89-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dcf89-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dcf89-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dcf89-114">Not supported.</span></span>|
|<span data-ttu-id="dcf89-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dcf89-115">Application</span></span>|<span data-ttu-id="dcf89-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dcf89-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dcf89-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dcf89-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenantGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dcf89-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dcf89-118">Optional query parameters</span></span>
<span data-ttu-id="dcf89-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="dcf89-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dcf89-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dcf89-120">Request headers</span></span>
|<span data-ttu-id="dcf89-121">Nome</span><span class="sxs-lookup"><span data-stu-id="dcf89-121">Name</span></span>|<span data-ttu-id="dcf89-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="dcf89-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="dcf89-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dcf89-123">Authorization</span></span>|<span data-ttu-id="dcf89-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dcf89-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcf89-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dcf89-126">Request body</span></span>
<span data-ttu-id="dcf89-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dcf89-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcf89-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcf89-128">Response</span></span>

<span data-ttu-id="dcf89-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [tenantGroup](../resources/managedtenants-tenantgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dcf89-129">If successful, this method returns a `200 OK` response code and a collection of [tenantGroup](../resources/managedtenants-tenantgroup.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dcf89-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dcf89-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dcf89-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dcf89-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="dcf89-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="dcf89-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tenantgroup"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantGroups
```
# <a name="c"></a>[<span data-ttu-id="dcf89-133">C#</span><span class="sxs-lookup"><span data-stu-id="dcf89-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tenantgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dcf89-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dcf89-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tenantgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dcf89-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dcf89-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tenantgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dcf89-136">Java</span><span class="sxs-lookup"><span data-stu-id="dcf89-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-tenantgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="dcf89-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="dcf89-137">Response</span></span>
><span data-ttu-id="dcf89-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="dcf89-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.tenantGroup)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/tenantGroups",
    "value": [
        {
            "id": "df7aed9c-c05a-4fc9-b958-64fafaed911d",
            "displayName": "Default",
            "allTenantsIncluded": true,
            "tenantIds": [],
            "managementIntents": [
                {
                    "managementIntentId": "586895ab-8a59-4b79-be25-b06949a819bb",
                    "managementIntentDisplayName": "Default Baseline",
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
            ],
            "managementActions": [
                {
                    "managementTemplateId": "12524106-036f-457f-b7a6-b003509d29c8",
                    "managementActionId": "eac82706-9f32-4274-ba5b-cf1f8ecf042b"
                },
                {
                    "managementTemplateId": "31d57d29-2d54-4074-84bd-51c008c2e6b2",
                    "managementActionId": "f104bb7f-4854-4209-ba09-c3788f9894c5"
                },
                {
                    "managementTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
                    "managementActionId": "4274db74-99c4-40be-bbeb-da4351136be2"
                },
                {
                    "managementTemplateId": "e5834405-43d2-4815-867d-3dd600308d1c",
                    "managementActionId": "e96a8cdb-0435-4808-9956-cf6b8ae77aa6"
                },
                {
                    "managementTemplateId": "b2d6d189-ea31-4cf8-b75e-41210c583127",
                    "managementActionId": "55f8da1a-4eec-4fb2-9c58-4c4b3cdf7222"
                },
                {
                    "managementTemplateId": "e2cadc41-a08f-45e7-8eb1-942d224dfb9a",
                    "managementActionId": "b22a4713-8428-4952-8cac-d48962ecbdc9"
                }
            ]
        }
    ]
}
```
