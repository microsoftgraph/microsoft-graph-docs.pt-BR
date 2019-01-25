---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharePointIds
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 22bf6b1101be9d60ff350e0b04f7627e2b8fb529
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524027"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="fba24-102">Tipo de recurso SharePointIds</span><span class="sxs-lookup"><span data-stu-id="fba24-102">SharePointIds resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fba24-103">O recurso **SharePointIds** agrupa os vários identificadores de um item armazenado em um site do SharePoint ou no OneDrive for Business em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="fba24-103">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="fba24-104">**Observação:** itens retornados do OneDrive pessoal não incluirão uma faceta **SharePointIds**.</span><span class="sxs-lookup"><span data-stu-id="fba24-104">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fba24-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fba24-105">JSON representation</span></span>

<span data-ttu-id="fba24-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="fba24-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "listId", "listItemId", "listItemUniqueId", "siteId", "siteUrl", "webId" ],
  "@odata.type": "microsoft.graph.sharepointIds"
}-->

```json
{
    "listId": "string",
    "listItemId": "string",
    "listItemUniqueId": "string",
    "siteId": "string",
    "siteUrl": "url",
    "tenantId": "string",
    "webId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="fba24-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fba24-107">Properties</span></span>

| <span data-ttu-id="fba24-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fba24-108">Property</span></span>         | <span data-ttu-id="fba24-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fba24-109">Type</span></span>         | <span data-ttu-id="fba24-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fba24-110">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="fba24-111">listId</span><span class="sxs-lookup"><span data-stu-id="fba24-111">listId</span></span>           | <span data-ttu-id="fba24-112">string</span><span class="sxs-lookup"><span data-stu-id="fba24-112">string</span></span>       | <span data-ttu-id="fba24-113">O identificador exclusivo (guid) para a lista do item no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fba24-113">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="fba24-114">listItemId</span><span class="sxs-lookup"><span data-stu-id="fba24-114">listItemId</span></span>       | <span data-ttu-id="fba24-115">string</span><span class="sxs-lookup"><span data-stu-id="fba24-115">string</span></span>       | <span data-ttu-id="fba24-116">Um identificador inteiro para o item na lista contida.</span><span class="sxs-lookup"><span data-stu-id="fba24-116">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="fba24-117">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="fba24-117">listItemUniqueId</span></span> | <span data-ttu-id="fba24-118">string</span><span class="sxs-lookup"><span data-stu-id="fba24-118">string</span></span>       | <span data-ttu-id="fba24-119">O identificador exclusivo (guid) do item dentro do OneDrive for Business ou de um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="fba24-119">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="fba24-120">siteId</span><span class="sxs-lookup"><span data-stu-id="fba24-120">siteId</span></span>           | <span data-ttu-id="fba24-121">string</span><span class="sxs-lookup"><span data-stu-id="fba24-121">string</span></span>       | <span data-ttu-id="fba24-122">O identificador exclusivo (guid) do conjunto de sites do item (SPSite).</span><span class="sxs-lookup"><span data-stu-id="fba24-122">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="fba24-123">siteUrl</span><span class="sxs-lookup"><span data-stu-id="fba24-123">siteUrl</span></span>          | <span data-ttu-id="fba24-124">string (url)</span><span class="sxs-lookup"><span data-stu-id="fba24-124">string (url)</span></span> | <span data-ttu-id="fba24-125">A URL do SharePoint do site que contém o item.</span><span class="sxs-lookup"><span data-stu-id="fba24-125">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="fba24-126">tenantId</span><span class="sxs-lookup"><span data-stu-id="fba24-126">tenantId</span></span>         | <span data-ttu-id="fba24-127">string</span><span class="sxs-lookup"><span data-stu-id="fba24-127">string</span></span>       | <span data-ttu-id="fba24-128">O identificador exclusivo (guid) de aluguel.</span><span class="sxs-lookup"><span data-stu-id="fba24-128">The unique identifier (guid) for the tenancy.</span></span>
| <span data-ttu-id="fba24-129">webId</span><span class="sxs-lookup"><span data-stu-id="fba24-129">webId</span></span>            | <span data-ttu-id="fba24-130">string</span><span class="sxs-lookup"><span data-stu-id="fba24-130">string</span></span>       | <span data-ttu-id="fba24-131">O identificador exclusivo (guid) do site do item (SPWeb).</span><span class="sxs-lookup"><span data-stu-id="fba24-131">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="fba24-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="fba24-132">Remarks</span></span>

<span data-ttu-id="fba24-133">Para saber mais sobre as facetas de um **driveItem**, confira [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="fba24-133">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharepointids.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
