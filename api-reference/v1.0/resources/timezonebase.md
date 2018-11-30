---
title: Tipo de recurso timeZoneBase
description: A representação básica de um fuso horário.
ms.openlocfilehash: 18df657ab561163b64bcf224f8902f2ba7e0039c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005527"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="12cf8-103">Tipo de recurso timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="12cf8-103">timeZoneBase resource type</span></span>

<span data-ttu-id="12cf8-104">A representação básica de um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="12cf8-104">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="12cf8-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="12cf8-105">Properties</span></span>
| <span data-ttu-id="12cf8-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12cf8-106">Property</span></span>     | <span data-ttu-id="12cf8-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="12cf8-107">Type</span></span>   |<span data-ttu-id="12cf8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="12cf8-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="12cf8-109">name</span><span class="sxs-lookup"><span data-stu-id="12cf8-109">name</span></span> | <span data-ttu-id="12cf8-110">string</span><span class="sxs-lookup"><span data-stu-id="12cf8-110">string</span></span> | <span data-ttu-id="12cf8-111">O nome de um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="12cf8-111">The name of a time zone.</span></span> <span data-ttu-id="12cf8-112">Pode ser o nome de um fuso horário padrão como "Hora Padrão do Havaí Aleuta" ou "Fuso Horário Personalizado" para um fuso horário personalizado.</span><span class="sxs-lookup"><span data-stu-id="12cf8-112">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="12cf8-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="12cf8-113">JSON representation</span></span>

<span data-ttu-id="12cf8-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="12cf8-114">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->