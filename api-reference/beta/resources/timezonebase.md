---
title: Tipo de recurso timeZoneBase
description: A representação básica de um fuso horário.
localization_priority: Normal
ms.openlocfilehash: 9fc07961aaa475980309d8c843b613da8b42e448
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523011"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="f4ff4-103">Tipo de recurso timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="f4ff4-103">timeZoneBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4ff4-104">A representação básica de um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="f4ff4-104">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="f4ff4-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4ff4-105">Properties</span></span>
| <span data-ttu-id="f4ff4-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4ff4-106">Property</span></span>     | <span data-ttu-id="f4ff4-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4ff4-107">Type</span></span>   |<span data-ttu-id="f4ff4-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4ff4-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f4ff4-109">nome</span><span class="sxs-lookup"><span data-stu-id="f4ff4-109">name</span></span> | <span data-ttu-id="f4ff4-110">string</span><span class="sxs-lookup"><span data-stu-id="f4ff4-110">string</span></span> | <span data-ttu-id="f4ff4-111">O nome de um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="f4ff4-111">The name of a time zone.</span></span> <span data-ttu-id="f4ff4-112">Pode ser o nome de um fuso horário padrão como "Hora Padrão do Havaí Aleuta" ou "Fuso Horário Personalizado" para um fuso horário personalizado.</span><span class="sxs-lookup"><span data-stu-id="f4ff4-112">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="f4ff4-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4ff4-113">JSON representation</span></span>

<span data-ttu-id="f4ff4-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f4ff4-114">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneBase"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timezonebase.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
