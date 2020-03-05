---
author: JeremyKelley
description: O recurso siteCollection fornece mais informações sobre um conjunto de sites.
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 240f0b804e8b87c0dc3aae1e03a46be3527bed22
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520538"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="5ec24-103">Recurso SiteCollection</span><span class="sxs-lookup"><span data-stu-id="5ec24-103">SiteCollection resource</span></span>

<span data-ttu-id="5ec24-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5ec24-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ec24-105">O recurso **siteCollection** fornece mais informações sobre um conjunto de sites.</span><span class="sxs-lookup"><span data-stu-id="5ec24-105">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="5ec24-106">Se um recurso [**site**](site.md) tem uma propriedade **siteCollection** não nula e, em seguida, o site é um site raiz do conjunto de sites.</span><span class="sxs-lookup"><span data-stu-id="5ec24-106">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ec24-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5ec24-107">JSON representation</span></span>

<span data-ttu-id="5ec24-108">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5ec24-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "dataLocationCode", "root"
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

## <a name="properties"></a><span data-ttu-id="5ec24-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5ec24-109">Properties</span></span>

| <span data-ttu-id="5ec24-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="5ec24-110">Property name</span></span>        | <span data-ttu-id="5ec24-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ec24-111">Type</span></span>     | <span data-ttu-id="5ec24-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ec24-112">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="5ec24-113">**hostname**</span><span class="sxs-lookup"><span data-stu-id="5ec24-113">**hostname**</span></span>         | <span data-ttu-id="5ec24-114">string</span><span class="sxs-lookup"><span data-stu-id="5ec24-114">string</span></span>   | <span data-ttu-id="5ec24-p101">O nome do host do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5ec24-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="5ec24-117">**dataLocationCode**</span><span class="sxs-lookup"><span data-stu-id="5ec24-117">**dataLocationCode**</span></span> | <span data-ttu-id="5ec24-118">string</span><span class="sxs-lookup"><span data-stu-id="5ec24-118">string</span></span>   | <span data-ttu-id="5ec24-119">O código de região geográfica para onde esse conjunto de sites reside.</span><span class="sxs-lookup"><span data-stu-id="5ec24-119">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="5ec24-120">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5ec24-120">Read-only.</span></span>
| <span data-ttu-id="5ec24-121">**root**</span><span class="sxs-lookup"><span data-stu-id="5ec24-121">**root**</span></span>             | <span data-ttu-id="5ec24-122">[root][]</span><span class="sxs-lookup"><span data-stu-id="5ec24-122">[root][]</span></span> | <span data-ttu-id="5ec24-123">Se presente, indica que esse é um conjunto de sites raiz no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5ec24-123">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="5ec24-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5ec24-124">Read-only.</span></span>

[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
