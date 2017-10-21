---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
ms.openlocfilehash: 6b36f3a0c2d958081f1b5663231a541f2e8a000f
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="sitecollection-resource"></a><span data-ttu-id="e1427-102">Recurso SiteCollection</span><span class="sxs-lookup"><span data-stu-id="e1427-102">SiteCollection resource</span></span>

<span data-ttu-id="e1427-103">O recurso **siteCollection** fornece mais informações sobre um conjunto de sites.</span><span class="sxs-lookup"><span data-stu-id="e1427-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="e1427-104">Se um recurso [**site**](site.md) tem uma propriedade **siteCollection** não nula e, em seguida, o site é um site raiz do conjunto de sites.</span><span class="sxs-lookup"><span data-stu-id="e1427-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1427-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1427-105">JSON representation</span></span>

<span data-ttu-id="e1427-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1427-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.siteCollection"
}-->

```json
{
  "hostname": "contoso.sharepoint.com"
}
```

## <a name="properties"></a><span data-ttu-id="e1427-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1427-107">Properties</span></span>

| <span data-ttu-id="e1427-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="e1427-108">Property name</span></span> | <span data-ttu-id="e1427-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1427-109">Type</span></span>    | <span data-ttu-id="e1427-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1427-110">Description</span></span>                                                                                                                  |
|:--------------|:--------|:---------------------------------------------------
| <span data-ttu-id="e1427-111">**hostname**</span><span class="sxs-lookup"><span data-stu-id="e1427-111">**hostname**</span></span>  | <span data-ttu-id="e1427-112">string</span><span class="sxs-lookup"><span data-stu-id="e1427-112">string</span></span>  | <span data-ttu-id="e1427-p101">O hostname do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e1427-p101">The hostname for the site collection. Read-only.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Facets/SiteCollection"
}-->
