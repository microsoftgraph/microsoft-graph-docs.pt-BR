---
title: Tipo de recurso timeZoneBase
description: A representação básica de um fuso horário.
localization_priority: Normal
ms.openlocfilehash: 8d968b8177da942c1b8940618c8ba965c362c914
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341866"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="d20e4-103">Tipo de recurso timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="d20e4-103">timeZoneBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d20e4-104">A representação básica de um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="d20e4-104">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="d20e4-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d20e4-105">Properties</span></span>
| <span data-ttu-id="d20e4-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d20e4-106">Property</span></span>     | <span data-ttu-id="d20e4-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d20e4-107">Type</span></span>   |<span data-ttu-id="d20e4-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d20e4-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d20e4-109">name</span><span class="sxs-lookup"><span data-stu-id="d20e4-109">name</span></span> | <span data-ttu-id="d20e4-110">string</span><span class="sxs-lookup"><span data-stu-id="d20e4-110">string</span></span> | <span data-ttu-id="d20e4-111">O nome de um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="d20e4-111">The name of a time zone.</span></span> <span data-ttu-id="d20e4-112">Pode ser o nome de um fuso horário padrão como "Hora Padrão do Havaí Aleuta" ou "Fuso Horário Personalizado" para um fuso horário personalizado.</span><span class="sxs-lookup"><span data-stu-id="d20e4-112">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="d20e4-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d20e4-113">JSON representation</span></span>

<span data-ttu-id="d20e4-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d20e4-114">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
