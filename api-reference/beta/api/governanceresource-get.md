---
title: Obter Entidadegovernanceresource
description: Recupere as propriedades e os relacionamentos de um objeto Entidadegovernanceresource.
localization_priority: Normal
ms.openlocfilehash: be24fb8822101f7a67a5bd60f1fe018cf1a08f6b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463926"
---
# <a name="get-governanceresource"></a><span data-ttu-id="ece77-103">Obter Entidadegovernanceresource</span><span class="sxs-lookup"><span data-stu-id="ece77-103">Get governanceResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ece77-104">Recupere as propriedades e os relacionamentos de um objeto [entidadegovernanceresource](../resources/governanceresource.md) .</span><span class="sxs-lookup"><span data-stu-id="ece77-104">Retrieve the properties and relationships of a [governanceResource](../resources/governanceresource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ece77-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ece77-105">Permissions</span></span>
<span data-ttu-id="ece77-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ece77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ece77-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ece77-108">Permission type</span></span>      | <span data-ttu-id="ece77-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="ece77-109">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ece77-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ece77-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ece77-111">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="ece77-111">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="ece77-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ece77-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ece77-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ece77-113">Not supported.</span></span>    |
|<span data-ttu-id="ece77-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ece77-114">Application</span></span> | <span data-ttu-id="ece77-115">PrivilegedAccess. ReadWrite. AzureResources</span><span class="sxs-lookup"><span data-stu-id="ece77-115">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="ece77-116">Além do escopo de permissão, essa API exige que o solicitante tenha pelo menos uma atribuição de função no recurso.</span><span class="sxs-lookup"><span data-stu-id="ece77-116">Besides the permission scope, this API requires the requestor to have at least one role assignment on the resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="ece77-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ece77-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedAccess/azureResources/resources/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ece77-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ece77-118">Optional query parameters</span></span>
<span data-ttu-id="ece77-119">Este método **só** oferece `$select` suporte `$expand` a [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ece77-119">This method **only** supports  `$select` and `$expand` [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ece77-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ece77-120">Request headers</span></span>
| <span data-ttu-id="ece77-121">Nome</span><span class="sxs-lookup"><span data-stu-id="ece77-121">Name</span></span>      |<span data-ttu-id="ece77-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ece77-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ece77-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ece77-123">Authorization</span></span>  | <span data-ttu-id="ece77-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="ece77-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ece77-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ece77-125">Request body</span></span>
<span data-ttu-id="ece77-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ece77-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ece77-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ece77-127">Response</span></span>
<span data-ttu-id="ece77-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [entidadegovernanceresource](../resources/governanceresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ece77-128">If successful, this method returns a `200 OK` response code and [governanceResource](../resources/governanceresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ece77-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ece77-129">Example</span></span>
<span data-ttu-id="ece77-130">Este exemplo mostra como obter os detalhes da assinatura Wingtip Toys-prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span><span class="sxs-lookup"><span data-stu-id="ece77-130">This example shows how to get the details of the subscription Wingtip Toys - Prod (e5e7d29d-5465-45ac-885f-4716a5ee74b5).</span></span>
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}-->
##### <a name="request"></a><span data-ttu-id="ece77-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ece77-131">Request</span></span>
```http
GET https://graph.microsoft.com/beta/privilegedAccess/azureResources/resources/e5e7d29d-5465-45ac-885f-4716a5ee74b5
```
##### <a name="response"></a><span data-ttu-id="ece77-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ece77-132">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 459

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceResources/$entity",
    "id": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
    "externalId": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",
    "type": "subscription",
    "displayName": "Wingtip Toys - Prod",
    "status": "Active",
    "registeredDateTime": "2018-04-05T22:30:37.13Z",
    "registeredRoot": "/subscriptions/38ab2ccc-3747-4567-b36b-9478f5602f0d",    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceresource-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
