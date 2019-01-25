---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 865fc21691eb37811300caaf675b123d1a544ac0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528127"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="da060-102">Recurso SiteCollection</span><span class="sxs-lookup"><span data-stu-id="da060-102">SiteCollection resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da060-103">O recurso **siteCollection** fornece mais informações sobre um conjunto de sites.</span><span class="sxs-lookup"><span data-stu-id="da060-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="da060-104">Se um recurso [**site**](site.md) tem uma propriedade **siteCollection** não nula e, em seguida, o site é um site raiz do conjunto de sites.</span><span class="sxs-lookup"><span data-stu-id="da060-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="da060-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da060-105">JSON representation</span></span>

<span data-ttu-id="da060-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="da060-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="da060-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da060-107">Properties</span></span>

| <span data-ttu-id="da060-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="da060-108">Property name</span></span>        | <span data-ttu-id="da060-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="da060-109">Type</span></span>     | <span data-ttu-id="da060-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="da060-110">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="da060-111">**hostname**</span><span class="sxs-lookup"><span data-stu-id="da060-111">**hostname**</span></span>         | <span data-ttu-id="da060-112">string</span><span class="sxs-lookup"><span data-stu-id="da060-112">string</span></span>   | <span data-ttu-id="da060-p101">O nome do host do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="da060-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="da060-115">**dataLocationCode**</span><span class="sxs-lookup"><span data-stu-id="da060-115">**dataLocationCode**</span></span> | <span data-ttu-id="da060-116">string</span><span class="sxs-lookup"><span data-stu-id="da060-116">string</span></span>   | <span data-ttu-id="da060-117">O código de região geográfica para onde esse conjunto de sites reside.</span><span class="sxs-lookup"><span data-stu-id="da060-117">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="da060-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="da060-118">Read-only.</span></span>
| <span data-ttu-id="da060-119">**root**</span><span class="sxs-lookup"><span data-stu-id="da060-119">**root**</span></span>             | <span data-ttu-id="da060-120">[root][]</span><span class="sxs-lookup"><span data-stu-id="da060-120">[root][]</span></span> | <span data-ttu-id="da060-121">Se presente, indica que este é um conjunto de sites raiz no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="da060-121">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="da060-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="da060-122">Read-only.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/sitecollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
