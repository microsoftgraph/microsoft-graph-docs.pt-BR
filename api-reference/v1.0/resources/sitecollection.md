---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.openlocfilehash: c366c39a71e952521425d9eb08fab7c77a9a3415
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809979"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="5a9ef-102">Recurso SiteCollection</span><span class="sxs-lookup"><span data-stu-id="5a9ef-102">SiteCollection resource</span></span>

<span data-ttu-id="5a9ef-103">O recurso **siteCollection** fornece mais informações sobre um conjunto de sites.</span><span class="sxs-lookup"><span data-stu-id="5a9ef-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="5a9ef-104">Se um recurso [**site**](site.md) tem uma propriedade **siteCollection** não nula e, em seguida, o site é um site raiz do conjunto de sites.</span><span class="sxs-lookup"><span data-stu-id="5a9ef-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a9ef-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a9ef-105">JSON representation</span></span>

<span data-ttu-id="5a9ef-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5a9ef-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="5a9ef-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5a9ef-107">Properties</span></span>

| <span data-ttu-id="5a9ef-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="5a9ef-108">Property name</span></span>        | <span data-ttu-id="5a9ef-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a9ef-109">Type</span></span>     | <span data-ttu-id="5a9ef-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a9ef-110">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="5a9ef-111">**hostname**</span><span class="sxs-lookup"><span data-stu-id="5a9ef-111">**hostname**</span></span>         | <span data-ttu-id="5a9ef-112">string</span><span class="sxs-lookup"><span data-stu-id="5a9ef-112">string</span></span>   | <span data-ttu-id="5a9ef-p101">O nome do host do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5a9ef-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="5a9ef-115">**root**</span><span class="sxs-lookup"><span data-stu-id="5a9ef-115">**root**</span></span>             | <span data-ttu-id="5a9ef-116">[root][]</span><span class="sxs-lookup"><span data-stu-id="5a9ef-116">[root][]</span></span> | <span data-ttu-id="5a9ef-117">Se presente, indica que este é um conjunto de sites raiz no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5a9ef-117">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="5a9ef-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="5a9ef-118">Read-only.</span></span>

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
