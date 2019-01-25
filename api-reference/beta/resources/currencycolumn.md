---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: CurrencyColumn
localization_priority: Normal
ms.openlocfilehash: c89d709c93eeee0003d193d620166f8abffd9d41
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524496"
---
# <a name="currencycolumn-resource-type"></a><span data-ttu-id="e82d9-102">Tipo de recurso CurrencyColumn</span><span class="sxs-lookup"><span data-stu-id="e82d9-102">CurrencyColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e82d9-103">**currencyColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna representam moeda.</span><span class="sxs-lookup"><span data-stu-id="e82d9-103">The **currencyColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values represent currency.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e82d9-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e82d9-104">JSON representation</span></span>

<span data-ttu-id="e82d9-105">Aqui está uma representação JSON de um recurso **currencyColumn**.</span><span class="sxs-lookup"><span data-stu-id="e82d9-105">Here is a JSON representation of a **currencyColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.currencyColumn" } -->

```json
{
  "locale": "en-us"
}
```

## <a name="properties"></a><span data-ttu-id="e82d9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e82d9-106">Properties</span></span>

| <span data-ttu-id="e82d9-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="e82d9-107">Property name</span></span> | <span data-ttu-id="e82d9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e82d9-108">Type</span></span>   | <span data-ttu-id="e82d9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e82d9-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="e82d9-110">**locale**</span><span class="sxs-lookup"><span data-stu-id="e82d9-110">**locale**</span></span>    | <span data-ttu-id="e82d9-111">string</span><span class="sxs-lookup"><span data-stu-id="e82d9-111">string</span></span> | <span data-ttu-id="e82d9-112">Especifica a localidade da qual o símbolo de moeda deverá ser inferido.</span><span class="sxs-lookup"><span data-stu-id="e82d9-112">Specifies the locale from which to infer the currency symbol.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/CurrencyColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/currencycolumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
