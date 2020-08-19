---
title: Tipo de recurso timeZoneBase
description: A representação básica de um fuso horário.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: a587070c32c85881ddf40d3f9cb2e64d5dd4aa50
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808505"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="5cf4e-103">Tipo de recurso timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="5cf4e-103">timeZoneBase resource type</span></span>

<span data-ttu-id="5cf4e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cf4e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5cf4e-105">A representação básica de um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="5cf4e-105">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="5cf4e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5cf4e-106">Properties</span></span>
| <span data-ttu-id="5cf4e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5cf4e-107">Property</span></span>     | <span data-ttu-id="5cf4e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5cf4e-108">Type</span></span>   |<span data-ttu-id="5cf4e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cf4e-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5cf4e-110">nome</span><span class="sxs-lookup"><span data-stu-id="5cf4e-110">name</span></span> | <span data-ttu-id="5cf4e-111">string</span><span class="sxs-lookup"><span data-stu-id="5cf4e-111">string</span></span> | <span data-ttu-id="5cf4e-112">O nome de um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="5cf4e-112">The name of a time zone.</span></span> <span data-ttu-id="5cf4e-113">Pode ser o nome de um fuso horário padrão como "Hora Padrão do Havaí Aleuta" ou "Fuso Horário Personalizado" para um fuso horário personalizado.</span><span class="sxs-lookup"><span data-stu-id="5cf4e-113">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="5cf4e-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5cf4e-114">JSON representation</span></span>

<span data-ttu-id="5cf4e-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5cf4e-115">Here is a JSON representation of the resource.</span></span>

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
