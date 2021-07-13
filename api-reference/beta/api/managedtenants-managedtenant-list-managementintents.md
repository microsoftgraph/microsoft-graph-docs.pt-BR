---
title: Gerenciamento de listaIntents
description: Obter uma lista dos objetos managementIntent e suas propriedades.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: a4aa3b605495b590148af09dafc14ff8a4edd491
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402105"
---
# <a name="list-managementintents"></a><span data-ttu-id="8c1bd-103">Gerenciamento de listaIntents</span><span class="sxs-lookup"><span data-stu-id="8c1bd-103">List managementIntents</span></span>
<span data-ttu-id="8c1bd-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="8c1bd-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c1bd-105">Obter uma lista dos [objetos managementIntent](../resources/managedtenants-managementintent.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="8c1bd-105">Get a list of the [managementIntent](../resources/managedtenants-managementintent.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c1bd-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8c1bd-106">Permissions</span></span>
<span data-ttu-id="8c1bd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c1bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c1bd-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8c1bd-109">Permission type</span></span>|<span data-ttu-id="8c1bd-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8c1bd-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c1bd-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8c1bd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8c1bd-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c1bd-112">ManagedTenants.Read.All, ManagedTenants.ReadWrite.All</span></span>|
|<span data-ttu-id="8c1bd-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8c1bd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c1bd-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c1bd-114">Not supported.</span></span>|
|<span data-ttu-id="8c1bd-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8c1bd-115">Application</span></span>|<span data-ttu-id="8c1bd-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8c1bd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c1bd-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8c1bd-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managementIntents
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8c1bd-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8c1bd-118">Optional query parameters</span></span>
<span data-ttu-id="8c1bd-119">Este método dá suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$apply` , , , , , , e `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="8c1bd-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8c1bd-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8c1bd-120">Request headers</span></span>
|<span data-ttu-id="8c1bd-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8c1bd-121">Name</span></span>|<span data-ttu-id="8c1bd-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c1bd-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="8c1bd-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8c1bd-123">Authorization</span></span>|<span data-ttu-id="8c1bd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8c1bd-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c1bd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8c1bd-126">Request body</span></span>
<span data-ttu-id="8c1bd-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8c1bd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c1bd-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c1bd-128">Response</span></span>

<span data-ttu-id="8c1bd-129">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos managementIntent](../resources/managedtenants-managementintent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8c1bd-129">If successful, this method returns a `200 OK` response code and a collection of [managementIntent](../resources/managedtenants-managementintent.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8c1bd-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8c1bd-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8c1bd-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8c1bd-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_managementintent"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementIntents
```


### <a name="response"></a><span data-ttu-id="8c1bd-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="8c1bd-132">Response</span></span>
><span data-ttu-id="8c1bd-133">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8c1bd-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.managementIntent)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managementIntents",
    "value": [
        {
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
    ]
}
```
