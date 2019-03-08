---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharePointIds
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c9f4c3dc54b9eee6cc1ab24058e3fe238fed89a3
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480597"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="a5199-102">Tipo de recurso SharePointIds</span><span class="sxs-lookup"><span data-stu-id="a5199-102">SharePointIds resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5199-103">O recurso **SharePointIds** agrupa os vários identificadores de um item armazenado em um site do SharePoint ou no OneDrive for Business em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="a5199-103">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="a5199-104">**Observação:** itens retornados do OneDrive pessoal não incluirão uma faceta **SharePointIds**.</span><span class="sxs-lookup"><span data-stu-id="a5199-104">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5199-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a5199-105">JSON representation</span></span>

<span data-ttu-id="a5199-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="a5199-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="a5199-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a5199-107">Properties</span></span>

| <span data-ttu-id="a5199-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5199-108">Property</span></span>         | <span data-ttu-id="a5199-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5199-109">Type</span></span>         | <span data-ttu-id="a5199-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5199-110">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="a5199-111">listId</span><span class="sxs-lookup"><span data-stu-id="a5199-111">listId</span></span>           | <span data-ttu-id="a5199-112">string</span><span class="sxs-lookup"><span data-stu-id="a5199-112">string</span></span>       | <span data-ttu-id="a5199-113">O identificador exclusivo (guid) para a lista do item no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a5199-113">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="a5199-114">listItemId</span><span class="sxs-lookup"><span data-stu-id="a5199-114">listItemId</span></span>       | <span data-ttu-id="a5199-115">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5199-115">string</span></span>       | <span data-ttu-id="a5199-116">Um identificador inteiro para o item na lista contida.</span><span class="sxs-lookup"><span data-stu-id="a5199-116">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="a5199-117">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="a5199-117">listItemUniqueId</span></span> | <span data-ttu-id="a5199-118">string</span><span class="sxs-lookup"><span data-stu-id="a5199-118">string</span></span>       | <span data-ttu-id="a5199-119">O identificador exclusivo (guid) do item dentro do OneDrive for Business ou de um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a5199-119">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="a5199-120">siteId</span><span class="sxs-lookup"><span data-stu-id="a5199-120">siteId</span></span>           | <span data-ttu-id="a5199-121">string</span><span class="sxs-lookup"><span data-stu-id="a5199-121">string</span></span>       | <span data-ttu-id="a5199-122">O identificador exclusivo (guid) do conjunto de sites do item (SPSite).</span><span class="sxs-lookup"><span data-stu-id="a5199-122">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="a5199-123">siteUrl</span><span class="sxs-lookup"><span data-stu-id="a5199-123">siteUrl</span></span>          | <span data-ttu-id="a5199-124">string (url)</span><span class="sxs-lookup"><span data-stu-id="a5199-124">string (url)</span></span> | <span data-ttu-id="a5199-125">A URL do SharePoint do site que contém o item.</span><span class="sxs-lookup"><span data-stu-id="a5199-125">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="a5199-126">tenantId</span><span class="sxs-lookup"><span data-stu-id="a5199-126">tenantId</span></span>         | <span data-ttu-id="a5199-127">string</span><span class="sxs-lookup"><span data-stu-id="a5199-127">string</span></span>       | <span data-ttu-id="a5199-128">O identificador exclusivo (GUID) da locação.</span><span class="sxs-lookup"><span data-stu-id="a5199-128">The unique identifier (guid) for the tenancy.</span></span>
| <span data-ttu-id="a5199-129">webId</span><span class="sxs-lookup"><span data-stu-id="a5199-129">webId</span></span>            | <span data-ttu-id="a5199-130">string</span><span class="sxs-lookup"><span data-stu-id="a5199-130">string</span></span>       | <span data-ttu-id="a5199-131">O identificador exclusivo (guid) do site do item (SPWeb).</span><span class="sxs-lookup"><span data-stu-id="a5199-131">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="a5199-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="a5199-132">Remarks</span></span>

<span data-ttu-id="a5199-133">Para saber mais sobre as facetas de um **driveItem**, confira [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="a5199-133">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



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
