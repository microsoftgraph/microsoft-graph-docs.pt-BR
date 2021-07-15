---
title: Gerenciamento de listaActionTenantDeploymentStatus
description: Obter uma lista dos objetos managementActionTenantDeploymentStatus e suas propriedades.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: adc102b8c292efe8b054c00922f3625cc3e75b1f
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441923"
---
# <a name="list-managementactiontenantdeploymentstatus"></a><span data-ttu-id="6c152-103">Gerenciamento de listaActionTenantDeploymentStatus</span><span class="sxs-lookup"><span data-stu-id="6c152-103">List managementActionTenantDeploymentStatus</span></span>
<span data-ttu-id="6c152-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="6c152-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c152-105">Obter uma lista dos [objetos managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="6c152-105">Get a list of the [managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c152-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="6c152-106">Permissions</span></span>
<span data-ttu-id="6c152-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c152-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c152-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c152-109">Permission type</span></span>|<span data-ttu-id="6c152-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6c152-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c152-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c152-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6c152-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c152-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="6c152-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c152-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c152-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c152-114">Not supported.</span></span>|
|<span data-ttu-id="6c152-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c152-115">Application</span></span>|<span data-ttu-id="6c152-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c152-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c152-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c152-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6c152-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6c152-118">Optional query parameters</span></span>
<span data-ttu-id="6c152-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="6c152-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c152-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c152-120">Request headers</span></span>
|<span data-ttu-id="6c152-121">Nome</span><span class="sxs-lookup"><span data-stu-id="6c152-121">Name</span></span>|<span data-ttu-id="6c152-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c152-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6c152-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c152-123">Authorization</span></span>|<span data-ttu-id="6c152-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6c152-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c152-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c152-126">Request body</span></span>
<span data-ttu-id="6c152-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6c152-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c152-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c152-128">Response</span></span>

<span data-ttu-id="6c152-129">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c152-129">If successful, this method returns a `200 OK` response code and a collection of [managementActionTenantDeploymentStatus](../resources/managedtenants-managementactiontenantdeploymentstatus.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6c152-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6c152-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6c152-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c152-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6c152-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c152-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_managementactiontenantdeploymentstatus"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses
```
# <a name="c"></a>[<span data-ttu-id="6c152-133">C#</span><span class="sxs-lookup"><span data-stu-id="6c152-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-managementactiontenantdeploymentstatus-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c152-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c152-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-managementactiontenantdeploymentstatus-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c152-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c152-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-managementactiontenantdeploymentstatus-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6c152-136">Java</span><span class="sxs-lookup"><span data-stu-id="6c152-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-managementactiontenantdeploymentstatus-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6c152-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c152-137">Response</span></span>
><span data-ttu-id="6c152-138">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6c152-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.managementActionTenantDeploymentStatus)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses",
    "value": [
        {
            "id": "df7aed9c-c05a-4fc9-b958-64fafaed911d_34298981-4fc8-4974-9486-c8909ed1521b",
            "tenantGroupId": "df7aed9c-c05a-4fc9-b958-64fafaed911d",
            "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
            "statuses": [
                {
                    "managementTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
                    "managementActionId": "4274db74-99c4-40be-bbeb-da4351136be2",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "fcb7ace7-3ea6-4474-912a-00ee78554445",
                            "status": "completed",
                            "deployedPolicyId": "949e8893-68fb-4c9d-b8a0-13c229a7e397",
                            "lastDeploymentDateTime": "2021-06-22T04:09:20.3054223Z",
                            "error": null
                        }
                    ]
                },
                {
                    "managementTemplateId": "31d57d29-2d54-4074-84bd-51c008c2e6b2",
                    "managementActionId": "f104bb7f-4854-4209-ba09-c3788f9894c5",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "00a9a585-f51c-4b68-b4f5-f0c3165df8ac",
                            "status": "completed",
                            "deployedPolicyId": "19a8d6a6-d87e-4059-85b3-c73bfc5cea15",
                            "lastDeploymentDateTime": "2021-06-22T17:01:44.851214Z",
                            "error": null
                        }
                    ]
                }
            ]
        },
        {
            "id": "df7aed9c-c05a-4fc9-b958-64fafaed911d_38227791-a88b-4fcc-81c5-58cf77668320",
            "tenantGroupId": "df7aed9c-c05a-4fc9-b958-64fafaed911d",
            "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
            "statuses": [
                {
                    "managementTemplateId": "12524106-036f-457f-b7a6-b003509d29c8",
                    "managementActionId": "eac82706-9f32-4274-ba5b-cf1f8ecf042b",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "7fff5ebb-10bd-4493-b0bb-2d0cf6172f16",
                            "status": "completed",
                            "deployedPolicyId": "062107b4-236d-465a-ae62-3bb4bd31f276",
                            "lastDeploymentDateTime": "2021-06-17T13:19:47.3003079Z",
                            "error": null
                        }
                    ]
                },
                {
                    "managementTemplateId": "b2d6d189-ea31-4cf8-b75e-41210c583127",
                    "managementActionId": "55f8da1a-4eec-4fb2-9c58-4c4b3cdf7222",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "4a1c5d34-c2f7-4fd5-a7b5-4bedd95bb8f9",
                            "status": "completed",
                            "deployedPolicyId": "606cf367-2075-40c4-a587-7914b6d83dc7",
                            "lastDeploymentDateTime": "2021-06-17T15:21:17.5296126Z",
                            "error": null
                        }
                    ]
                },
                {
                    "managementTemplateId": "31d57d29-2d54-4074-84bd-51c008c2e6b2",
                    "managementActionId": "f104bb7f-4854-4209-ba09-c3788f9894c5",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "00a9a585-f51c-4b68-b4f5-f0c3165df8ac",
                            "status": "completed",
                            "deployedPolicyId": "60148b3e-39a2-4c0c-95a6-375a939aa756",
                            "lastDeploymentDateTime": "2021-06-22T05:54:42.7087204Z",
                            "error": null
                        }
                    ]
                },
                {
                    "managementTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
                    "managementActionId": "4274db74-99c4-40be-bbeb-da4351136be2",
                    "status": "riskAccepted",
                    "workloadActionDeploymentStatuses": []
                },
                {
                    "managementTemplateId": "e5834405-43d2-4815-867d-3dd600308d1c",
                    "managementActionId": "e96a8cdb-0435-4808-9956-cf6b8ae77aa6",
                    "status": "toAddress",
                    "workloadActionDeploymentStatuses": []
                }
            ]
        },
        {
            "id": "df7aed9c-c05a-4fc9-b958-64fafaed911d_4d262a25-c70a-430b-9e8e-46c31dec116b",
            "tenantGroupId": "df7aed9c-c05a-4fc9-b958-64fafaed911d",
            "tenantId": "4d262a25-c70a-430b-9e8e-46c31dec116b",
            "statuses": [
                {
                    "managementTemplateId": "31d57d29-2d54-4074-84bd-51c008c2e6b2",
                    "managementActionId": "f104bb7f-4854-4209-ba09-c3788f9894c5",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "00a9a585-f51c-4b68-b4f5-f0c3165df8ac",
                            "status": "completed",
                            "deployedPolicyId": "aee50adb-9445-44a8-baaf-7d16b388d708",
                            "lastDeploymentDateTime": "2021-06-18T20:21:00.0934112Z",
                            "error": null
                        }
                    ]
                },
                {
                    "managementTemplateId": "12524106-036f-457f-b7a6-b003509d29c8",
                    "managementActionId": "eac82706-9f32-4274-ba5b-cf1f8ecf042b",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "7fff5ebb-10bd-4493-b0bb-2d0cf6172f16",
                            "status": "completed",
                            "deployedPolicyId": "67635cbb-6519-44dd-bf7f-fd8752d1339b",
                            "lastDeploymentDateTime": "2021-07-09T18:53:07.113328Z",
                            "error": null
                        }
                    ]
                },
                {
                    "managementTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
                    "managementActionId": "4274db74-99c4-40be-bbeb-da4351136be2",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "fcb7ace7-3ea6-4474-912a-00ee78554445",
                            "status": "completed",
                            "deployedPolicyId": "f296e4d5-7b4a-4c7b-977f-cd4e5bbbc0ea",
                            "lastDeploymentDateTime": "2021-07-09T20:12:33.6197104Z",
                            "error": null
                        }
                    ]
                }
            ]
        },
        {
            "id": "df7aed9c-c05a-4fc9-b958-64fafaed911d_791fae7d-ffda-4187-ba69-14ed55bdb026",
            "tenantGroupId": "df7aed9c-c05a-4fc9-b958-64fafaed911d",
            "tenantId": "791fae7d-ffda-4187-ba69-14ed55bdb026",
            "statuses": [
                {
                    "managementTemplateId": "12524106-036f-457f-b7a6-b003509d29c8",
                    "managementActionId": "eac82706-9f32-4274-ba5b-cf1f8ecf042b",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "7fff5ebb-10bd-4493-b0bb-2d0cf6172f16",
                            "status": "completed",
                            "deployedPolicyId": "2e628607-5908-4dea-89c3-61438dd77805",
                            "lastDeploymentDateTime": "2021-06-17T05:14:12.671197Z",
                            "error": null
                        }
                    ]
                },
                {
                    "managementTemplateId": "21230aa5-d5a9-4403-b179-baf2de242aca",
                    "managementActionId": "4274db74-99c4-40be-bbeb-da4351136be2",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "fcb7ace7-3ea6-4474-912a-00ee78554445",
                            "status": "completed",
                            "deployedPolicyId": "deebefee-f378-4d2e-ab1a-a7f2bf1a010e",
                            "lastDeploymentDateTime": "2021-06-17T05:15:08.801992Z",
                            "error": null
                        }
                    ]
                },
                {
                    "managementTemplateId": "e5834405-43d2-4815-867d-3dd600308d1c",
                    "managementActionId": "e96a8cdb-0435-4808-9956-cf6b8ae77aa6",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "6a3ad0bc-5d7e-4a49-a105-c559aa4633e1",
                            "status": "completed",
                            "deployedPolicyId": "e14428f4-9890-4f6b-8416-ec40d9a59646",
                            "lastDeploymentDateTime": "2021-06-17T05:15:57.5564366Z",
                            "error": null
                        }
                    ]
                },
                {
                    "managementTemplateId": "b2d6d189-ea31-4cf8-b75e-41210c583127",
                    "managementActionId": "55f8da1a-4eec-4fb2-9c58-4c4b3cdf7222",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "4a1c5d34-c2f7-4fd5-a7b5-4bedd95bb8f9",
                            "status": "completed",
                            "deployedPolicyId": "220bbe5d-2167-4ba1-8c7d-67bd56b0e068",
                            "lastDeploymentDateTime": "2021-06-17T05:16:35.1968434Z",
                            "error": null
                        }
                    ]
                },
                {
                    "managementTemplateId": "31d57d29-2d54-4074-84bd-51c008c2e6b2",
                    "managementActionId": "f104bb7f-4854-4209-ba09-c3788f9894c5",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "00a9a585-f51c-4b68-b4f5-f0c3165df8ac",
                            "status": "completed",
                            "deployedPolicyId": "50553bd7-560e-4c0e-9c80-78f4ae9560e5",
                            "lastDeploymentDateTime": "2021-06-17T05:17:46.2079328Z",
                            "error": null
                        }
                    ]
                },
                {
                    "managementTemplateId": "e2cadc41-a08f-45e7-8eb1-942d224dfb9a",
                    "managementActionId": "b22a4713-8428-4952-8cac-d48962ecbdc9",
                    "status": "completed",
                    "workloadActionDeploymentStatuses": [
                        {
                            "actionId": "46b80b42-06c7-45b4-b6fb-aa0aecace87b",
                            "status": "completed",
                            "deployedPolicyId": null,
                            "lastDeploymentDateTime": "2021-06-17T05:18:16.7581968Z",
                            "error": null
                        }
                    ]
                }
            ]
        }
    ]
}
```
