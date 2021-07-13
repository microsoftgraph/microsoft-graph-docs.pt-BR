---
title: Listar tenantGroups
description: Obter uma lista dos objetos tenantGroup e suas propriedades.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 11bb89e594308fad86f61c2d9d1d422e684c48ee
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402104"
---
# <a name="list-tenantgroups"></a><span data-ttu-id="cf47f-103">Listar tenantGroups</span><span class="sxs-lookup"><span data-stu-id="cf47f-103">List tenantGroups</span></span>
<span data-ttu-id="cf47f-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="cf47f-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf47f-105">Obter uma lista dos objetos [tenantGroup](../resources/managedtenants-tenantgroup.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="cf47f-105">Get a list of the [tenantGroup](../resources/managedtenants-tenantgroup.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf47f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cf47f-106">Permissions</span></span>
<span data-ttu-id="cf47f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf47f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf47f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf47f-109">Permission type</span></span>|<span data-ttu-id="cf47f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cf47f-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf47f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf47f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cf47f-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf47f-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="cf47f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf47f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf47f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf47f-114">Not supported.</span></span>|
|<span data-ttu-id="cf47f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf47f-115">Application</span></span>|<span data-ttu-id="cf47f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf47f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf47f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf47f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenantGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cf47f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cf47f-118">Optional query parameters</span></span>
<span data-ttu-id="cf47f-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="cf47f-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf47f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf47f-120">Request headers</span></span>
|<span data-ttu-id="cf47f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="cf47f-121">Name</span></span>|<span data-ttu-id="cf47f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf47f-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cf47f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf47f-123">Authorization</span></span>|<span data-ttu-id="cf47f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf47f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf47f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf47f-126">Request body</span></span>
<span data-ttu-id="cf47f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cf47f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf47f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf47f-128">Response</span></span>

<span data-ttu-id="cf47f-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de objetos [tenantGroup](../resources/managedtenants-tenantgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf47f-129">If successful, this method returns a `200 OK` response code and a collection of [tenantGroup](../resources/managedtenants-tenantgroup.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cf47f-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cf47f-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cf47f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf47f-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_tenantgroup"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantGroups
```


### <a name="response"></a><span data-ttu-id="cf47f-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf47f-132">Response</span></span>
><span data-ttu-id="cf47f-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cf47f-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
