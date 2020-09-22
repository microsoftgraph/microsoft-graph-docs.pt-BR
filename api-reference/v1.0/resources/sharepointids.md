---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharePointIds
localization_priority: Normal
ms.prod: sharepoint
description: O recurso SharePointIds agrupa os vários identificadores de um item armazenado em um site do SharePoint ou no OneDrive for Business em uma única estrutura.
doc_type: resourcePageType
ms.openlocfilehash: 4289f2b4785ca06588722ee12c0e6620b092ddce
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094166"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="493a0-103">Tipo de recurso SharePointIds</span><span class="sxs-lookup"><span data-stu-id="493a0-103">SharePointIds resource type</span></span>

<span data-ttu-id="493a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="493a0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="493a0-105">O recurso **SharePointIds** agrupa os vários identificadores de um item armazenado em um site do SharePoint ou no OneDrive for Business em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="493a0-105">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="493a0-106">**Observação:** itens retornados do OneDrive pessoal não incluirão uma faceta **SharePointIds**.</span><span class="sxs-lookup"><span data-stu-id="493a0-106">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="493a0-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="493a0-107">JSON representation</span></span>

<span data-ttu-id="493a0-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="493a0-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="493a0-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="493a0-109">Properties</span></span>

| <span data-ttu-id="493a0-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="493a0-110">Property</span></span>         | <span data-ttu-id="493a0-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="493a0-111">Type</span></span>         | <span data-ttu-id="493a0-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="493a0-112">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="493a0-113">listId</span><span class="sxs-lookup"><span data-stu-id="493a0-113">listId</span></span>           | <span data-ttu-id="493a0-114">string</span><span class="sxs-lookup"><span data-stu-id="493a0-114">string</span></span>       | <span data-ttu-id="493a0-115">O identificador exclusivo (guid) para a lista do item no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="493a0-115">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="493a0-116">listItemId</span><span class="sxs-lookup"><span data-stu-id="493a0-116">listItemId</span></span>       | <span data-ttu-id="493a0-117">string</span><span class="sxs-lookup"><span data-stu-id="493a0-117">string</span></span>       | <span data-ttu-id="493a0-118">Um identificador inteiro para o item na lista contida.</span><span class="sxs-lookup"><span data-stu-id="493a0-118">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="493a0-119">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="493a0-119">listItemUniqueId</span></span> | <span data-ttu-id="493a0-120">string</span><span class="sxs-lookup"><span data-stu-id="493a0-120">string</span></span>       | <span data-ttu-id="493a0-121">O identificador exclusivo (guid) do item dentro do OneDrive for Business ou de um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="493a0-121">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="493a0-122">siteId</span><span class="sxs-lookup"><span data-stu-id="493a0-122">siteId</span></span>           | <span data-ttu-id="493a0-123">string</span><span class="sxs-lookup"><span data-stu-id="493a0-123">string</span></span>       | <span data-ttu-id="493a0-124">O identificador exclusivo (guid) do conjunto de sites do item (SPSite).</span><span class="sxs-lookup"><span data-stu-id="493a0-124">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="493a0-125">siteUrl</span><span class="sxs-lookup"><span data-stu-id="493a0-125">siteUrl</span></span>          | <span data-ttu-id="493a0-126">string (url)</span><span class="sxs-lookup"><span data-stu-id="493a0-126">string (url)</span></span> | <span data-ttu-id="493a0-127">A URL do SharePoint do site que contém o item.</span><span class="sxs-lookup"><span data-stu-id="493a0-127">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="493a0-128">tenantId</span><span class="sxs-lookup"><span data-stu-id="493a0-128">tenantId</span></span>         | <span data-ttu-id="493a0-129">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="493a0-129">string</span></span>       | <span data-ttu-id="493a0-130">O identificador exclusivo (GUID) da locação.</span><span class="sxs-lookup"><span data-stu-id="493a0-130">The unique identifier (guid) for the tenancy.</span></span>
| <span data-ttu-id="493a0-131">webId</span><span class="sxs-lookup"><span data-stu-id="493a0-131">webId</span></span>            | <span data-ttu-id="493a0-132">string</span><span class="sxs-lookup"><span data-stu-id="493a0-132">string</span></span>       | <span data-ttu-id="493a0-133">O identificador exclusivo (guid) do site do item (SPWeb).</span><span class="sxs-lookup"><span data-stu-id="493a0-133">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="493a0-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="493a0-134">Remarks</span></span>

<span data-ttu-id="493a0-135">Para saber mais sobre as facetas de um **driveItem**, confira [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="493a0-135">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds"
} -->

