---
title: tipo de recurso plannerPlanContextDetails
description: O recurso **plannerPlanContextDetails** contém informações adicionais sobre um plannerPlanContext.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 025e5b1623333d0235ae83e061e30247a3d130f6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505939"
---
# <a name="plannerplancontextdetails-resource-type"></a><span data-ttu-id="2f975-103">tipo de recurso plannerPlanContextDetails</span><span class="sxs-lookup"><span data-stu-id="2f975-103">plannerPlanContextDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f975-104">O recurso **plannerPlanContextDetails** contém informações adicionais sobre um [plannerPlanContext](plannerplancontext.md).</span><span class="sxs-lookup"><span data-stu-id="2f975-104">The **plannerPlanContextDetails** resource contains additional information about a [plannerPlanContext](plannerplancontext.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2f975-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2f975-105">Properties</span></span>
| <span data-ttu-id="2f975-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f975-106">Property</span></span>     | <span data-ttu-id="2f975-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f975-107">Type</span></span>   |<span data-ttu-id="2f975-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f975-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f975-109">url</span><span class="sxs-lookup"><span data-stu-id="2f975-109">url</span></span>|<span data-ttu-id="2f975-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f975-110">String</span></span>|<span data-ttu-id="2f975-111">URL da experiência do usuário representada pelo [plannerPlanContext](plannerplancontext.md)associado.</span><span class="sxs-lookup"><span data-stu-id="2f975-111">URL of the user experience represented by the associated [plannerPlanContext](plannerplancontext.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2f975-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2f975-112">JSON representation</span></span>

<span data-ttu-id="2f975-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2f975-113">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextDetails"
}-->

```json
{
  "url": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplancontextdetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
