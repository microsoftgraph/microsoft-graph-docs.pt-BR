---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e9525882b08aaae5500ce23a4b54e95d0b0e0d65
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583694"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="7c930-102">Recurso SiteCollection</span><span class="sxs-lookup"><span data-stu-id="7c930-102">SiteCollection resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c930-103">O recurso **siteCollection** fornece mais informações sobre um conjunto de sites.</span><span class="sxs-lookup"><span data-stu-id="7c930-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="7c930-104">Se um recurso [**site**](site.md) tem uma propriedade **siteCollection** não nula e, em seguida, o site é um site raiz do conjunto de sites.</span><span class="sxs-lookup"><span data-stu-id="7c930-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c930-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7c930-105">JSON representation</span></span>

<span data-ttu-id="7c930-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7c930-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="7c930-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7c930-107">Properties</span></span>

| <span data-ttu-id="7c930-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="7c930-108">Property name</span></span>        | <span data-ttu-id="7c930-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c930-109">Type</span></span>     | <span data-ttu-id="7c930-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c930-110">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="7c930-111">**hostname**</span><span class="sxs-lookup"><span data-stu-id="7c930-111">**hostname**</span></span>         | <span data-ttu-id="7c930-112">string</span><span class="sxs-lookup"><span data-stu-id="7c930-112">string</span></span>   | <span data-ttu-id="7c930-p101">O nome do host do conjunto de sites. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7c930-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="7c930-115">**dataLocationCode**</span><span class="sxs-lookup"><span data-stu-id="7c930-115">**dataLocationCode**</span></span> | <span data-ttu-id="7c930-116">string</span><span class="sxs-lookup"><span data-stu-id="7c930-116">string</span></span>   | <span data-ttu-id="7c930-117">O código de região geográfica para onde esse conjunto de sites reside.</span><span class="sxs-lookup"><span data-stu-id="7c930-117">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="7c930-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7c930-118">Read-only.</span></span>
| <span data-ttu-id="7c930-119">**root**</span><span class="sxs-lookup"><span data-stu-id="7c930-119">**root**</span></span>             | <span data-ttu-id="7c930-120">[root][]</span><span class="sxs-lookup"><span data-stu-id="7c930-120">[root][]</span></span> | <span data-ttu-id="7c930-121">Se presente, indica que esse é um conjunto de sites raiz no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7c930-121">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="7c930-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7c930-122">Read-only.</span></span>

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
