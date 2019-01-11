---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharePointIds
localization_priority: Normal
ms.openlocfilehash: 6c67c45b333ead1d427c5b15ddd4ed5925b84eac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807809"
---
# <a name="sharepointids-resource-type"></a><span data-ttu-id="e099e-102">Tipo de recurso SharePointIds</span><span class="sxs-lookup"><span data-stu-id="e099e-102">SharePointIds resource type</span></span>

> <span data-ttu-id="e099e-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e099e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e099e-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e099e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e099e-105">O recurso **SharePointIds** agrupa os vários identificadores de um item armazenado em um site do SharePoint ou no OneDrive for Business em uma única estrutura.</span><span class="sxs-lookup"><span data-stu-id="e099e-105">The **SharePointIds** resource groups the various identifiers for an item stored in a SharePoint site or OneDrive for Business into a single structure.</span></span>

<span data-ttu-id="e099e-106">**Observação:** itens retornados do OneDrive pessoal não incluirão uma faceta **SharePointIds**.</span><span class="sxs-lookup"><span data-stu-id="e099e-106">**Note:** items returned from OneDrive personal will not include a **SharePointIds** facet.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e099e-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e099e-107">JSON representation</span></span>

<span data-ttu-id="e099e-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="e099e-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="e099e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e099e-109">Properties</span></span>

| <span data-ttu-id="e099e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e099e-110">Property</span></span>         | <span data-ttu-id="e099e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e099e-111">Type</span></span>         | <span data-ttu-id="e099e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e099e-112">Description</span></span>
|:-----------------|:-------------|:-------------------------------------------
| <span data-ttu-id="e099e-113">listId</span><span class="sxs-lookup"><span data-stu-id="e099e-113">listId</span></span>           | <span data-ttu-id="e099e-114">string</span><span class="sxs-lookup"><span data-stu-id="e099e-114">string</span></span>       | <span data-ttu-id="e099e-115">O identificador exclusivo (guid) para a lista do item no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e099e-115">The unique identifier (guid) for the item's list in SharePoint.</span></span>
| <span data-ttu-id="e099e-116">listItemId</span><span class="sxs-lookup"><span data-stu-id="e099e-116">listItemId</span></span>       | <span data-ttu-id="e099e-117">string</span><span class="sxs-lookup"><span data-stu-id="e099e-117">string</span></span>       | <span data-ttu-id="e099e-118">Um identificador inteiro para o item na lista contida.</span><span class="sxs-lookup"><span data-stu-id="e099e-118">An integer identifier for the item within the containing list.</span></span>
| <span data-ttu-id="e099e-119">listItemUniqueId</span><span class="sxs-lookup"><span data-stu-id="e099e-119">listItemUniqueId</span></span> | <span data-ttu-id="e099e-120">string</span><span class="sxs-lookup"><span data-stu-id="e099e-120">string</span></span>       | <span data-ttu-id="e099e-121">O identificador exclusivo (guid) do item dentro do OneDrive for Business ou de um site do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e099e-121">The unique identifier (guid) for the item within OneDrive for Business or a SharePoint site.</span></span>
| <span data-ttu-id="e099e-122">siteId</span><span class="sxs-lookup"><span data-stu-id="e099e-122">siteId</span></span>           | <span data-ttu-id="e099e-123">string</span><span class="sxs-lookup"><span data-stu-id="e099e-123">string</span></span>       | <span data-ttu-id="e099e-124">O identificador exclusivo (guid) do conjunto de sites do item (SPSite).</span><span class="sxs-lookup"><span data-stu-id="e099e-124">The unique identifier (guid) for the item's site collection (SPSite).</span></span>
| <span data-ttu-id="e099e-125">siteUrl</span><span class="sxs-lookup"><span data-stu-id="e099e-125">siteUrl</span></span>          | <span data-ttu-id="e099e-126">string (url)</span><span class="sxs-lookup"><span data-stu-id="e099e-126">string (url)</span></span> | <span data-ttu-id="e099e-127">A URL do SharePoint do site que contém o item.</span><span class="sxs-lookup"><span data-stu-id="e099e-127">The SharePoint URL for the site that contains the item.</span></span>
| <span data-ttu-id="e099e-128">tenantId</span><span class="sxs-lookup"><span data-stu-id="e099e-128">tenantId</span></span>         | <span data-ttu-id="e099e-129">string</span><span class="sxs-lookup"><span data-stu-id="e099e-129">string</span></span>       | <span data-ttu-id="e099e-130">O identificador exclusivo (guid) de aluguel.</span><span class="sxs-lookup"><span data-stu-id="e099e-130">The unique identifier (guid) for the tenancy.</span></span>
| <span data-ttu-id="e099e-131">webId</span><span class="sxs-lookup"><span data-stu-id="e099e-131">webId</span></span>            | <span data-ttu-id="e099e-132">string</span><span class="sxs-lookup"><span data-stu-id="e099e-132">string</span></span>       | <span data-ttu-id="e099e-133">O identificador exclusivo (guid) do site do item (SPWeb).</span><span class="sxs-lookup"><span data-stu-id="e099e-133">The unique identifier (guid) for the item's site (SPWeb).</span></span>

## <a name="remarks"></a><span data-ttu-id="e099e-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="e099e-134">Remarks</span></span>

<span data-ttu-id="e099e-135">Para saber mais sobre as facetas de um **driveItem**, confira [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e099e-135">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds"
} -->
