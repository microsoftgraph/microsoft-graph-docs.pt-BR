---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
description: O recurso siteCollection fornece mais informações sobre um conjunto de sites.
doc_type: resourcePageType
ms.openlocfilehash: 27a534f2f9afe99a1a5abb1aee91b1b53b29566d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034157"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="a1c7b-103">Recurso SiteCollection</span><span class="sxs-lookup"><span data-stu-id="a1c7b-103">SiteCollection resource</span></span>

<span data-ttu-id="a1c7b-104">O recurso **siteCollection** fornece mais informações sobre um conjunto de sites.</span><span class="sxs-lookup"><span data-stu-id="a1c7b-104">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="a1c7b-105">Se um recurso [**site**](site.md) tem uma propriedade **siteCollection** não nula e, em seguida, o site é um site raiz do conjunto de sites.</span><span class="sxs-lookup"><span data-stu-id="a1c7b-105">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1c7b-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a1c7b-106">JSON representation</span></span>

<span data-ttu-id="a1c7b-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a1c7b-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.siteCollection"
}-->

```json
{
  "hostname": "contoso.sharepoint.com",
  "root": { "@odata.type": "microsoft.graph.root" }
}
```

## <a name="properties"></a><span data-ttu-id="a1c7b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a1c7b-108">Properties</span></span>

| <span data-ttu-id="a1c7b-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="a1c7b-109">Property name</span></span>        | <span data-ttu-id="a1c7b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1c7b-110">Type</span></span>     | <span data-ttu-id="a1c7b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1c7b-111">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="a1c7b-112">**hostname**</span><span class="sxs-lookup"><span data-stu-id="a1c7b-112">**hostname**</span></span>         | <span data-ttu-id="a1c7b-113">string</span><span class="sxs-lookup"><span data-stu-id="a1c7b-113">string</span></span>   | <span data-ttu-id="a1c7b-p101">O nome do host do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a1c7b-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="a1c7b-116">**root**</span><span class="sxs-lookup"><span data-stu-id="a1c7b-116">**root**</span></span>             | <span data-ttu-id="a1c7b-117">[root][]</span><span class="sxs-lookup"><span data-stu-id="a1c7b-117">[root][]</span></span> | <span data-ttu-id="a1c7b-118">Se presente, indica que esse é um conjunto de sites raiz no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a1c7b-118">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="a1c7b-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a1c7b-119">Read-only.</span></span>

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
