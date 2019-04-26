---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharePointIds
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 01e4c3087f9504255975ab28f935ceed8815b6b0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343090"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="7809f-102">Tipo de recurso SharePointIds</span><span class="sxs-lookup"><span data-stu-id="7809f-102">SharePointIds resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7809f-103">O recurso **SharePointIds** agrupa os vários identificadores de um item armazenado em um site do SharePoint ou no OneDrive for Business em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="7809f-103">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="7809f-104">**Observação:** itens retornados do OneDrive pessoal não incluirão uma faceta **SharePointIds**.</span><span class="sxs-lookup"><span data-stu-id="7809f-104">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7809f-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7809f-105">JSON representation</span></span>

<span data-ttu-id="7809f-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7809f-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="7809f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7809f-107">Properties</span></span>

| <span data-ttu-id="7809f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7809f-108">Property</span></span>         | <span data-ttu-id="7809f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7809f-109">Type</span></span>         | <span data-ttu-id="7809f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7809f-110">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="7809f-111">listId</span><span class="sxs-lookup"><span data-stu-id="7809f-111">listId</span></span>           | <span data-ttu-id="7809f-112">string</span><span class="sxs-lookup"><span data-stu-id="7809f-112">string</span></span>       | <span data-ttu-id="7809f-113">O identificador exclusivo (guid) para a lista do item no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7809f-113">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="7809f-114">listItemId</span><span class="sxs-lookup"><span data-stu-id="7809f-114">listItemId</span></span>       | <span data-ttu-id="7809f-115">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7809f-115">string</span></span>       | <span data-ttu-id="7809f-116">Um identificador inteiro para o item na lista contida.</span><span class="sxs-lookup"><span data-stu-id="7809f-116">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="7809f-117">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="7809f-117">listItemUniqueId</span></span> | <span data-ttu-id="7809f-118">string</span><span class="sxs-lookup"><span data-stu-id="7809f-118">string</span></span>       | <span data-ttu-id="7809f-119">O identificador exclusivo (guid) do item dentro do OneDrive for Business ou de um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7809f-119">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="7809f-120">siteId</span><span class="sxs-lookup"><span data-stu-id="7809f-120">siteId</span></span>           | <span data-ttu-id="7809f-121">string</span><span class="sxs-lookup"><span data-stu-id="7809f-121">string</span></span>       | <span data-ttu-id="7809f-122">O identificador exclusivo (guid) do conjunto de sites do item (SPSite).</span><span class="sxs-lookup"><span data-stu-id="7809f-122">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="7809f-123">siteUrl</span><span class="sxs-lookup"><span data-stu-id="7809f-123">siteUrl</span></span>          | <span data-ttu-id="7809f-124">string (url)</span><span class="sxs-lookup"><span data-stu-id="7809f-124">string (url)</span></span> | <span data-ttu-id="7809f-125">A URL do SharePoint do site que contém o item.</span><span class="sxs-lookup"><span data-stu-id="7809f-125">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="7809f-126">tenantId</span><span class="sxs-lookup"><span data-stu-id="7809f-126">tenantId</span></span>         | <span data-ttu-id="7809f-127">string</span><span class="sxs-lookup"><span data-stu-id="7809f-127">string</span></span>       | <span data-ttu-id="7809f-128">O identificador exclusivo (GUID) da locação.</span><span class="sxs-lookup"><span data-stu-id="7809f-128">The unique identifier (guid) for the tenancy.</span></span>
| <span data-ttu-id="7809f-129">webId</span><span class="sxs-lookup"><span data-stu-id="7809f-129">webId</span></span>            | <span data-ttu-id="7809f-130">string</span><span class="sxs-lookup"><span data-stu-id="7809f-130">string</span></span>       | <span data-ttu-id="7809f-131">O identificador exclusivo (guid) do site do item (SPWeb).</span><span class="sxs-lookup"><span data-stu-id="7809f-131">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="7809f-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="7809f-132">Remarks</span></span>

<span data-ttu-id="7809f-133">Para saber mais sobre as facetas de um **driveItem**, confira [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="7809f-133">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds",
  "suppressions": []
}
-->
