---
title: Obter governanceRoleDefinition
description: Recupere as propriedades e os relacionamentos de um governanceRoleDefinition.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: d9cf9f091581678da3b22585c75c163537bfe163
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991037"
---
# <a name="get-governanceroledefinition"></a><span data-ttu-id="78499-103">Obter governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="78499-103">Get governanceRoleDefinition</span></span>

<span data-ttu-id="78499-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78499-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78499-105">Recupere as propriedades e os relacionamentos de um [governanceRoleDefinition](../resources/governanceroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="78499-105">Retrieve the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="78499-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="78499-106">Permissions</span></span>
<span data-ttu-id="78499-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78499-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78499-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78499-109">Permission type</span></span>      | <span data-ttu-id="78499-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="78499-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78499-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78499-111">Delegated (work or school account)</span></span> | <span data-ttu-id="78499-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="78499-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="78499-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78499-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78499-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78499-114">Not supported.</span></span>    |
|<span data-ttu-id="78499-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78499-115">Application</span></span> | <span data-ttu-id="78499-116">PrivilegedAccess. Read. AzureResources</span><span class="sxs-lookup"><span data-stu-id="78499-116">PrivilegedAccess.Read.AzureResources</span></span> |

<span data-ttu-id="78499-117">Além do escopo de permissão, essa API exige que o solicitante tenha pelo menos uma atribuição de função no recurso ao qual o [governanceRoleDefinition](../resources/governanceroledefinition.md) pertence.</span><span class="sxs-lookup"><span data-stu-id="78499-117">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleDefinition](../resources/governanceroledefinition.md) belongs to.</span></span>

## <a name="http-request"></a><span data-ttu-id="78499-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78499-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions/{id}
GET /privilegedAccess/azureResources/roleDefinitions/{id}?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="78499-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="78499-119">Optional query parameters</span></span>
<span data-ttu-id="78499-120">Este **método não oferece suporte** aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="78499-120">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="78499-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78499-121">Request headers</span></span>
| <span data-ttu-id="78499-122">Nome</span><span class="sxs-lookup"><span data-stu-id="78499-122">Name</span></span>      |<span data-ttu-id="78499-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="78499-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="78499-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="78499-124">Authorization</span></span>  | <span data-ttu-id="78499-125">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="78499-125">Bearer {code}</span></span>|


## <a name="request-body"></a><span data-ttu-id="78499-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78499-126">Request body</span></span>
<span data-ttu-id="78499-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="78499-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="78499-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="78499-128">Response</span></span>
<span data-ttu-id="78499-129">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [governanceRoleDefinition](../resources/governanceroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78499-129">If successful, this method returns a `200 OK` response code and [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="78499-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78499-130">Example</span></span>
<span data-ttu-id="78499-131">Este exemplo mostra como obter detalhes da definição de função colaborador da zona DNS na assinatura Wingtip Toys-prod.</span><span class="sxs-lookup"><span data-stu-id="78499-131">This example shows how to get details of role definition DNS Zone Contributor in the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinition"
}-->
##### <a name="request"></a><span data-ttu-id="78499-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78499-132">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions/00efc9e0-1b96-4e9a-99a3-a3df0735cf88
```
##### <a name="response"></a><span data-ttu-id="78499-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="78499-133">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 174

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleDefinitions/$entity",
    "id": "00efc9e0-1b96-4e9a-99a3-a3df0735cf88",
    "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d/providers/Microsoft.Authorization/roleDefinitions/befefa01-2a29-4197-83a8-272ff33ce314",
    "templateId": "befefa01-2a29-4197-83a8-272ff33ce314",
    "displayName": "DNS Zone Contributor"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


