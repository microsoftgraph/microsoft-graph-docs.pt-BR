---
author: JeremyKelley
description: O recurso SharePointIds agrupa os vários identificadores de um item armazenado em um site do SharePoint ou no OneDrive for Business em uma única estrutura.
ms.date: 09/10/2017
title: SharePointIds
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: c7e18e43bcbe9c73500701577c752e7a30d47194
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965121"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="3ea35-103">Tipo de recurso SharePointIds</span><span class="sxs-lookup"><span data-stu-id="3ea35-103">SharePointIds resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ea35-104">O recurso **SharePointIds** agrupa os vários identificadores de um item armazenado em um site do SharePoint ou no OneDrive for Business em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="3ea35-104">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="3ea35-105">**Observação:** itens retornados do OneDrive pessoal não incluirão uma faceta **SharePointIds**.</span><span class="sxs-lookup"><span data-stu-id="3ea35-105">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ea35-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3ea35-106">JSON representation</span></span>

<span data-ttu-id="3ea35-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="3ea35-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="3ea35-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3ea35-108">Properties</span></span>

| <span data-ttu-id="3ea35-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ea35-109">Property</span></span>         | <span data-ttu-id="3ea35-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ea35-110">Type</span></span>         | <span data-ttu-id="3ea35-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ea35-111">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="3ea35-112">listId</span><span class="sxs-lookup"><span data-stu-id="3ea35-112">listId</span></span>           | <span data-ttu-id="3ea35-113">string</span><span class="sxs-lookup"><span data-stu-id="3ea35-113">string</span></span>       | <span data-ttu-id="3ea35-114">O identificador exclusivo (guid) para a lista do item no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3ea35-114">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="3ea35-115">listItemId</span><span class="sxs-lookup"><span data-stu-id="3ea35-115">listItemId</span></span>       | <span data-ttu-id="3ea35-116">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3ea35-116">string</span></span>       | <span data-ttu-id="3ea35-117">Um identificador inteiro para o item na lista contida.</span><span class="sxs-lookup"><span data-stu-id="3ea35-117">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="3ea35-118">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="3ea35-118">listItemUniqueId</span></span> | <span data-ttu-id="3ea35-119">string</span><span class="sxs-lookup"><span data-stu-id="3ea35-119">string</span></span>       | <span data-ttu-id="3ea35-120">O identificador exclusivo (guid) do item dentro do OneDrive for Business ou de um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3ea35-120">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="3ea35-121">siteId</span><span class="sxs-lookup"><span data-stu-id="3ea35-121">siteId</span></span>           | <span data-ttu-id="3ea35-122">string</span><span class="sxs-lookup"><span data-stu-id="3ea35-122">string</span></span>       | <span data-ttu-id="3ea35-123">O identificador exclusivo (guid) do conjunto de sites do item (SPSite).</span><span class="sxs-lookup"><span data-stu-id="3ea35-123">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="3ea35-124">siteUrl</span><span class="sxs-lookup"><span data-stu-id="3ea35-124">siteUrl</span></span>          | <span data-ttu-id="3ea35-125">string (url)</span><span class="sxs-lookup"><span data-stu-id="3ea35-125">string (url)</span></span> | <span data-ttu-id="3ea35-126">A URL do SharePoint do site que contém o item.</span><span class="sxs-lookup"><span data-stu-id="3ea35-126">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="3ea35-127">tenantId</span><span class="sxs-lookup"><span data-stu-id="3ea35-127">tenantId</span></span>         | <span data-ttu-id="3ea35-128">string</span><span class="sxs-lookup"><span data-stu-id="3ea35-128">string</span></span>       | <span data-ttu-id="3ea35-129">O identificador exclusivo (GUID) da locação.</span><span class="sxs-lookup"><span data-stu-id="3ea35-129">The unique identifier (guid) for the tenancy.</span></span>
| <span data-ttu-id="3ea35-130">webId</span><span class="sxs-lookup"><span data-stu-id="3ea35-130">webId</span></span>            | <span data-ttu-id="3ea35-131">string</span><span class="sxs-lookup"><span data-stu-id="3ea35-131">string</span></span>       | <span data-ttu-id="3ea35-132">O identificador exclusivo (guid) do site do item (SPWeb).</span><span class="sxs-lookup"><span data-stu-id="3ea35-132">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="3ea35-133">Comentários</span><span class="sxs-lookup"><span data-stu-id="3ea35-133">Remarks</span></span>

<span data-ttu-id="3ea35-134">Para saber mais sobre as facetas de um **driveItem**, confira [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="3ea35-134">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



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
