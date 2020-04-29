---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
description: O recurso siteCollection fornece mais informações sobre um conjunto de sites.
doc_type: resourcePageType
ms.openlocfilehash: f73505ead4ad060f81bdfe7e77099783a8ff0242
ms.sourcegitcommit: 9b507499fb1ec61b4de47f36f915ae29c8594459
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2020
ms.locfileid: "43934819"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="d62b8-103">Recurso SiteCollection</span><span class="sxs-lookup"><span data-stu-id="d62b8-103">SiteCollection resource</span></span>

<span data-ttu-id="d62b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d62b8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d62b8-105">O recurso **siteCollection** fornece mais informações sobre um conjunto de sites.</span><span class="sxs-lookup"><span data-stu-id="d62b8-105">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="d62b8-106">Se um recurso [**site**](site.md) tem uma propriedade **siteCollection** não nula e, em seguida, o site é um site raiz do conjunto de sites.</span><span class="sxs-lookup"><span data-stu-id="d62b8-106">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d62b8-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d62b8-107">JSON representation</span></span>

<span data-ttu-id="d62b8-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d62b8-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.siteCollection"
}-->

```json
{
  "hostname": "contoso.sharepoint.com",
  "dataLocationCode": "EUR",
  "root": { "@odata.type": "microsoft.graph.root" }
}
```

## <a name="properties"></a><span data-ttu-id="d62b8-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d62b8-109">Properties</span></span>

| <span data-ttu-id="d62b8-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="d62b8-110">Property name</span></span>        | <span data-ttu-id="d62b8-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d62b8-111">Type</span></span>     | <span data-ttu-id="d62b8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d62b8-112">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="d62b8-113">**hostname**</span><span class="sxs-lookup"><span data-stu-id="d62b8-113">**hostname**</span></span>         | <span data-ttu-id="d62b8-114">string</span><span class="sxs-lookup"><span data-stu-id="d62b8-114">string</span></span>   | <span data-ttu-id="d62b8-p101">O nome do host do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d62b8-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="d62b8-117">**dataLocationCode**</span><span class="sxs-lookup"><span data-stu-id="d62b8-117">**dataLocationCode**</span></span> | <span data-ttu-id="d62b8-118">string</span><span class="sxs-lookup"><span data-stu-id="d62b8-118">string</span></span>   | <span data-ttu-id="d62b8-119">O código de região geográfica para onde esse conjunto de sites reside.</span><span class="sxs-lookup"><span data-stu-id="d62b8-119">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="d62b8-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d62b8-120">Read-only.</span></span>
| <span data-ttu-id="d62b8-121">**root**</span><span class="sxs-lookup"><span data-stu-id="d62b8-121">**root**</span></span>             | <span data-ttu-id="d62b8-122">[root][]</span><span class="sxs-lookup"><span data-stu-id="d62b8-122">[root][]</span></span> | <span data-ttu-id="d62b8-123">Se presente, indica que esse é um conjunto de sites raiz no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d62b8-123">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="d62b8-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d62b8-124">Read-only.</span></span>

[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Facets/SiteCollection"
}-->
