---
title: Obter governanceRoleDefinition
description: Recupere as propriedades e os relacionamentos de um governanceRoleDefinition.
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 1c9eb59fd3ffaff3963db4f10139d123c6c154c6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954113"
---
# <a name="get-governanceroledefinition"></a><span data-ttu-id="9ac20-103">Obter governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9ac20-103">Get governanceRoleDefinition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ac20-104">Recupere as propriedades e os relacionamentos de um [governanceRoleDefinition](../resources/governanceroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9ac20-104">Retrieve the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9ac20-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9ac20-105">Permissions</span></span>
<span data-ttu-id="9ac20-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ac20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ac20-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ac20-108">Permission type</span></span>      | <span data-ttu-id="9ac20-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="9ac20-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ac20-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ac20-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9ac20-111">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="9ac20-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="9ac20-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ac20-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ac20-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ac20-113">Not supported.</span></span>    |
|<span data-ttu-id="9ac20-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ac20-114">Application</span></span> | <span data-ttu-id="9ac20-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ac20-115">Not supported.</span></span> |

<span data-ttu-id="9ac20-116">Além do escopo de permissão, essa API exige que o solicitante tenha pelo menos uma atribuição de função no recurso ao qual o [governanceRoleDefinition](../resources/governanceroledefinition.md) pertence.</span><span class="sxs-lookup"><span data-stu-id="9ac20-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleDefinition](../resources/governanceroledefinition.md) belongs to.</span></span>

## <a name="http-request"></a><span data-ttu-id="9ac20-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ac20-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions/{id}
GET /privilegedAccess/azureResources/roleDefinitions/{id}?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9ac20-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9ac20-118">Optional query parameters</span></span>
<span data-ttu-id="9ac20-119">Este método não \*\*\*\* oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9ac20-119">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ac20-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ac20-120">Request headers</span></span>
| <span data-ttu-id="9ac20-121">Nome</span><span class="sxs-lookup"><span data-stu-id="9ac20-121">Name</span></span>      |<span data-ttu-id="9ac20-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ac20-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9ac20-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ac20-123">Authorization</span></span>  | <span data-ttu-id="9ac20-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="9ac20-124">Bearer {code}</span></span>|


## <a name="request-body"></a><span data-ttu-id="9ac20-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ac20-125">Request body</span></span>
<span data-ttu-id="9ac20-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9ac20-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9ac20-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ac20-127">Response</span></span>
<span data-ttu-id="9ac20-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [governanceRoleDefinition](../resources/governanceroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9ac20-128">If successful, this method returns a `200 OK` response code and [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9ac20-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ac20-129">Example</span></span>
<span data-ttu-id="9ac20-130">Este exemplo mostra como obter detalhes da definição de função colaborador da zona DNS na assinatura Wingtip Toys-prod.</span><span class="sxs-lookup"><span data-stu-id="9ac20-130">This example shows how to get details of role definition DNS Zone Contributor in the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinition"
}-->
##### <a name="request"></a><span data-ttu-id="9ac20-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ac20-131">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions/00efc9e0-1b96-4e9a-99a3-a3df0735cf88
```
##### <a name="response"></a><span data-ttu-id="9ac20-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ac20-132">Response</span></span>
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
