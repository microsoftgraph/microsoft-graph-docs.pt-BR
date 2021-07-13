---
title: Listar tenantTags
description: Obter uma lista dos objetos tenantTag e suas propriedades.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: a277228444b527082360eb1fc9e3ad886dbe7b55
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402020"
---
# <a name="list-tenanttags"></a><span data-ttu-id="24e1a-103">Listar tenantTags</span><span class="sxs-lookup"><span data-stu-id="24e1a-103">List tenantTags</span></span>
<span data-ttu-id="24e1a-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="24e1a-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24e1a-105">Obter uma lista dos objetos [tenantTag](../resources/managedtenants-tenanttag.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="24e1a-105">Get a list of the [tenantTag](../resources/managedtenants-tenanttag.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="24e1a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="24e1a-106">Permissions</span></span>
<span data-ttu-id="24e1a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24e1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24e1a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24e1a-109">Permission type</span></span>|<span data-ttu-id="24e1a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="24e1a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24e1a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24e1a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="24e1a-112">ManagedTenants.Read.All, ManagedTenants.WriteRead.All</span><span class="sxs-lookup"><span data-stu-id="24e1a-112">ManagedTenants.Read.All, ManagedTenants.WriteRead.All</span></span>|
|<span data-ttu-id="24e1a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24e1a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24e1a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24e1a-114">Not supported.</span></span>|
|<span data-ttu-id="24e1a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24e1a-115">Application</span></span>|<span data-ttu-id="24e1a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24e1a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24e1a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24e1a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/tenantTags
```

## <a name="optional-query-parameters"></a><span data-ttu-id="24e1a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="24e1a-118">Optional query parameters</span></span>
<span data-ttu-id="24e1a-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$count` , , , , , e `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="24e1a-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="24e1a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24e1a-120">Request headers</span></span>
|<span data-ttu-id="24e1a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="24e1a-121">Name</span></span>|<span data-ttu-id="24e1a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="24e1a-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="24e1a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="24e1a-123">Authorization</span></span>|<span data-ttu-id="24e1a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24e1a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="24e1a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24e1a-126">Request body</span></span>
<span data-ttu-id="24e1a-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24e1a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24e1a-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="24e1a-128">Response</span></span>

<span data-ttu-id="24e1a-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos tenantTag](../resources/managedtenants-tenanttag.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24e1a-129">If successful, this method returns a `200 OK` response code and a collection of [tenantTag](../resources/managedtenants-tenanttag.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="24e1a-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="24e1a-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="24e1a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24e1a-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_tenanttag"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/tenantTags
```


### <a name="response"></a><span data-ttu-id="24e1a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="24e1a-132">Response</span></span>
><span data-ttu-id="24e1a-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="24e1a-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.tenantTag)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/tenantTags",
    "value": [
        {
            "id": "913391c0-5466-42b4-900d-0a7501399cb0",
            "displayName": "Onboarding",
            "description": "Tenants that we are currently onboarding",
            "properties": null,
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
        },
        {
            "id": "bfd883e8-10f3-40ee-994c-111fa1c5d1db",
            "displayName": "ExtendedSupport",
            "description": "Tenants that have purchased extended support.",
            "properties": null,
            "tenantIds": [
                "38227791-a88b-4fcc-81c5-58cf77668320",
                "4d262a25-c70a-430b-9e8e-46c31dec116b"
            ],
            "isDeleted": null,
            "createdDateTime": "2021-06-16T20:43:31.8917383Z",
            "createdByUserId": "43a2424c-0fa3-446d-bee9-4ab500bb1603",
            "lastActionDateTime": "2021-06-17T03:23:31.3531635Z",
            "lastActionByUserId": "248f617e-a6a7-4d31-922d-726c24074bb6",
            "tenants": [
                {
                    "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320"
                },
                {
                    "tenantId": "4d262a25-c70a-430b-9e8e-46c31dec116b"
                }
            ]
        }
    ]
}
```
