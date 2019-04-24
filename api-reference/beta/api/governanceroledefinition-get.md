---
title: Obter governanceRoleDefinition
description: Recupere as propriedades e os relacionamentos de um governanceRoleDefinition.
localization_priority: Normal
ms.openlocfilehash: e6a057816a8e07a355941f272325c30078327ab9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503044"
---
# <a name="get-governanceroledefinition"></a><span data-ttu-id="0ea8a-103">Obter governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="0ea8a-103">Get governanceRoleDefinition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ea8a-104">Recupere as propriedades e os relacionamentos de um [governanceRoleDefinition](../resources/governanceroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="0ea8a-104">Retrieve the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0ea8a-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0ea8a-105">Permissions</span></span>
<span data-ttu-id="0ea8a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ea8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ea8a-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ea8a-108">Permission type</span></span>      | <span data-ttu-id="0ea8a-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="0ea8a-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ea8a-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ea8a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0ea8a-111">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="0ea8a-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="0ea8a-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ea8a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ea8a-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ea8a-113">Not supported.</span></span>    |
|<span data-ttu-id="0ea8a-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ea8a-114">Application</span></span> | <span data-ttu-id="0ea8a-115">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="0ea8a-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="0ea8a-116">Além do escopo de permissão, essa API exige que o solicitante tenha pelo menos uma atribuição de função no recurso ao qual o [governanceRoleDefinition](../resources/governanceroledefinition.md) pertence.</span><span class="sxs-lookup"><span data-stu-id="0ea8a-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleDefinition](../resources/governanceroledefinition.md) belongs to.</span></span>

## <a name="http-request"></a><span data-ttu-id="0ea8a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ea8a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions/{id}
GET /privilegedAccess/azureResources/roleDefinitions/{id}?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0ea8a-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0ea8a-118">Optional query parameters</span></span>
<span data-ttu-id="0ea8a-119">Este método não \*\*\*\* oferece suporte aos [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0ea8a-119">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ea8a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ea8a-120">Request headers</span></span>
| <span data-ttu-id="0ea8a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0ea8a-121">Name</span></span>      |<span data-ttu-id="0ea8a-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ea8a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0ea8a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ea8a-123">Authorization</span></span>  | <span data-ttu-id="0ea8a-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="0ea8a-124">Bearer {code}</span></span>|


## <a name="request-body"></a><span data-ttu-id="0ea8a-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ea8a-125">Request body</span></span>
<span data-ttu-id="0ea8a-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0ea8a-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0ea8a-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ea8a-127">Response</span></span>
<span data-ttu-id="0ea8a-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [governanceRoleDefinition](../resources/governanceroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ea8a-128">If successful, this method returns a `200 OK` response code and [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0ea8a-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ea8a-129">Example</span></span>
<span data-ttu-id="0ea8a-130">Este exemplo mostra como obter detalhes da definição de função colaborador da zona DNS na assinatura Wingtip Toys-prod.</span><span class="sxs-lookup"><span data-stu-id="0ea8a-130">This example shows how to get details of role definition DNS Zone Contributor in the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinition"
}-->
##### <a name="request"></a><span data-ttu-id="0ea8a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ea8a-131">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions/00efc9e0-1b96-4e9a-99a3-a3df0735cf88
```
##### <a name="response"></a><span data-ttu-id="0ea8a-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ea8a-132">Response</span></span>
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
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroledefinition-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
