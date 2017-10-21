---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharePointIds
ms.openlocfilehash: 36636ead90d8b913de4328aea9b6252e82f30c26
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="b4f53-102">Tipo de recurso SharePointIds</span><span class="sxs-lookup"><span data-stu-id="b4f53-102">SharePointIds resource type</span></span>

<span data-ttu-id="b4f53-103">O recurso **SharePointIds** agrupa os vários identificadores de um item armazenado em um site do SharePoint ou no OneDrive for Business em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="b4f53-103">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="b4f53-104">**Observação:** itens retornados do OneDrive pessoal não incluirão uma faceta **SharePointIds**.</span><span class="sxs-lookup"><span data-stu-id="b4f53-104">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4f53-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b4f53-105">JSON representation</span></span>

<span data-ttu-id="b4f53-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b4f53-106">Here is a JSON representation of the resource</span></span>

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
    "webId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="b4f53-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b4f53-107">Properties</span></span>

| <span data-ttu-id="b4f53-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4f53-108">Property</span></span>         | <span data-ttu-id="b4f53-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4f53-109">Type</span></span>         | <span data-ttu-id="b4f53-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4f53-110">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="b4f53-111">listId</span><span class="sxs-lookup"><span data-stu-id="b4f53-111">listId</span></span>           | <span data-ttu-id="b4f53-112">string</span><span class="sxs-lookup"><span data-stu-id="b4f53-112">string</span></span>       | <span data-ttu-id="b4f53-113">O identificador exclusivo (guid) para a lista do item no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b4f53-113">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="b4f53-114">listItemId</span><span class="sxs-lookup"><span data-stu-id="b4f53-114">listItemId</span></span>       | <span data-ttu-id="b4f53-115">string</span><span class="sxs-lookup"><span data-stu-id="b4f53-115">string</span></span>       | <span data-ttu-id="b4f53-116">Um identificador inteiro para o item na lista contida.</span><span class="sxs-lookup"><span data-stu-id="b4f53-116">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="b4f53-117">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="b4f53-117">listItemUniqueId</span></span> | <span data-ttu-id="b4f53-118">string</span><span class="sxs-lookup"><span data-stu-id="b4f53-118">string</span></span>       | <span data-ttu-id="b4f53-119">O identificador exclusivo (guid) do item dentro do OneDrive for Business ou de um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b4f53-119">The unique identifier (guid) for the item within OneDrive for Busienss or a SharePoint site.</span></span>
| <span data-ttu-id="b4f53-120">siteId</span><span class="sxs-lookup"><span data-stu-id="b4f53-120">siteId</span></span>           | <span data-ttu-id="b4f53-121">string</span><span class="sxs-lookup"><span data-stu-id="b4f53-121">string</span></span>       | <span data-ttu-id="b4f53-122">O identificador exclusivo (guid) do conjunto de sites do item (SPSite).</span><span class="sxs-lookup"><span data-stu-id="b4f53-122">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="b4f53-123">siteUrl</span><span class="sxs-lookup"><span data-stu-id="b4f53-123">siteUrl</span></span>          | <span data-ttu-id="b4f53-124">string (url)</span><span class="sxs-lookup"><span data-stu-id="b4f53-124">string (url)</span></span> | <span data-ttu-id="b4f53-125">A URL do SharePoint do site que contém o item.</span><span class="sxs-lookup"><span data-stu-id="b4f53-125">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="b4f53-126">webId</span><span class="sxs-lookup"><span data-stu-id="b4f53-126">webId</span></span>            | <span data-ttu-id="b4f53-127">string</span><span class="sxs-lookup"><span data-stu-id="b4f53-127">string</span></span>       | <span data-ttu-id="b4f53-128">O identificador exclusivo (guid) do site do item (SPWeb).</span><span class="sxs-lookup"><span data-stu-id="b4f53-128">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="b4f53-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="b4f53-129">Remarks</span></span>

<span data-ttu-id="b4f53-130">Para saber mais sobre as facetas de um **driveItem**, confira [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="b4f53-130">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds"
} -->
