---
title: Obter tenantGroup
description: Leia as propriedades e as relações de um objeto tenantGroup.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: e01fae422015e6acf6f6d3fdbd8468ed929454a4
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401961"
---
# <a name="get-tenantgroup"></a><span data-ttu-id="f6fc9-103">Obter tenantGroup</span><span class="sxs-lookup"><span data-stu-id="f6fc9-103">Get tenantGroup</span></span>
<span data-ttu-id="f6fc9-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="f6fc9-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6fc9-105">Leia as propriedades e as relações de um [objeto tenantGroup.](../resources/managedtenants-tenantgroup.md)</span><span class="sxs-lookup"><span data-stu-id="f6fc9-105">Read the properties and relationships of a [tenantGroup](../resources/managedtenants-tenantgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6fc9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f6fc9-106">Permissions</span></span>
<span data-ttu-id="f6fc9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6fc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6fc9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f6fc9-109">Permission type</span></span>|<span data-ttu-id="f6fc9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f6fc9-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6fc9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f6fc9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f6fc9-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6fc9-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="f6fc9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f6fc9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6fc9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6fc9-114">Not supported.</span></span>|
|<span data-ttu-id="f6fc9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f6fc9-115">Application</span></span>|<span data-ttu-id="f6fc9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f6fc9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6fc9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f6fc9-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenantGroups/{tenantGroupId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6fc9-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f6fc9-118">Optional query parameters</span></span>
<span data-ttu-id="f6fc9-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="f6fc9-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6fc9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f6fc9-120">Request headers</span></span>
|<span data-ttu-id="f6fc9-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f6fc9-121">Name</span></span>|<span data-ttu-id="f6fc9-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6fc9-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f6fc9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f6fc9-123">Authorization</span></span>|<span data-ttu-id="f6fc9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f6fc9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6fc9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f6fc9-126">Request body</span></span>
<span data-ttu-id="f6fc9-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f6fc9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6fc9-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6fc9-128">Response</span></span>

<span data-ttu-id="f6fc9-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [tenantGroup](../resources/managedtenants-tenantgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f6fc9-129">If successful, this method returns a `200 OK` response code and a [tenantGroup](../resources/managedtenants-tenantgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f6fc9-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f6fc9-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f6fc9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f6fc9-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tenantgroup"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantGroups/{tenantGroupId}
```


### <a name="response"></a><span data-ttu-id="f6fc9-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f6fc9-132">Response</span></span>
><span data-ttu-id="f6fc9-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f6fc9-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.tenantGroup"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/tenantGroups/$entity",
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
```
