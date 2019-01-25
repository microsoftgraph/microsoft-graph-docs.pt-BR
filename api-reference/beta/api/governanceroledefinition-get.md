---
title: Obter governanceRoleDefinition
description: Recupere as propriedades e relacionamentos de um governanceRoleDefinition.
localization_priority: Normal
ms.openlocfilehash: e6a057816a8e07a355941f272325c30078327ab9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511923"
---
# <a name="get-governanceroledefinition"></a><span data-ttu-id="9d607-103">Obter governanceRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="9d607-103">Get governanceRoleDefinition</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d607-104">Recupere as propriedades e relacionamentos de um [governanceRoleDefinition](../resources/governanceroledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="9d607-104">Retrieve the properties and relationships of a [governanceRoleDefinition](../resources/governanceroledefinition.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9d607-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9d607-105">Permissions</span></span>
<span data-ttu-id="9d607-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d607-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d607-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d607-108">Permission type</span></span>      | <span data-ttu-id="9d607-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="9d607-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d607-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d607-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9d607-111">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="9d607-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="9d607-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d607-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d607-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d607-113">Not supported.</span></span>    |
|<span data-ttu-id="9d607-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9d607-114">Application</span></span> | <span data-ttu-id="9d607-115">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="9d607-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="9d607-116">Além do escopo de permissão, essa API requer o solicitante ter pelo menos uma atribuição do recurso, que pertence a [governanceRoleDefinition](../resources/governanceroledefinition.md) .</span><span class="sxs-lookup"><span data-stu-id="9d607-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource, which the [governanceRoleDefinition](../resources/governanceroledefinition.md) belongs to.</span></span>

## <a name="http-request"></a><span data-ttu-id="9d607-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d607-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{resourceId}/roleDefinitions/{id}
GET /privilegedAccess/azureResources/roleDefinitions/{id}?$filter=resourceId+eq+'{resourceId}'
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9d607-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9d607-118">Optional query parameters</span></span>
<span data-ttu-id="9d607-119">Esse método não **suporte os [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta** .</span><span class="sxs-lookup"><span data-stu-id="9d607-119">This method does **not** support the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d607-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9d607-120">Request headers</span></span>
| <span data-ttu-id="9d607-121">Nome</span><span class="sxs-lookup"><span data-stu-id="9d607-121">Name</span></span>      |<span data-ttu-id="9d607-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d607-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9d607-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9d607-123">Authorization</span></span>  | <span data-ttu-id="9d607-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="9d607-124">Bearer {code}</span></span>|


## <a name="request-body"></a><span data-ttu-id="9d607-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d607-125">Request body</span></span>
<span data-ttu-id="9d607-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9d607-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9d607-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d607-127">Response</span></span>
<span data-ttu-id="9d607-128">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [governanceRoleDefinition](../resources/governanceroledefinition.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d607-128">If successful, this method returns a `200 OK` response code and [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9d607-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9d607-129">Example</span></span>
<span data-ttu-id="9d607-130">Este exemplo mostra como obter os detalhes da definição de função de Colaborador de zona de DNS na assinatura Wingtip Toys - produção.</span><span class="sxs-lookup"><span data-stu-id="9d607-130">This example shows how to get details of role definition DNS Zone Contributor in the subscription Wingtip Toys - Prod.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinition"
}-->
##### <a name="request"></a><span data-ttu-id="9d607-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d607-131">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5/roleDefinitions/00efc9e0-1b96-4e9a-99a3-a3df0735cf88
```
##### <a name="response"></a><span data-ttu-id="9d607-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d607-132">Response</span></span>
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
