---
title: Tipo de recurso timeZoneBase
description: A representação básica de um fuso horário.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: a5ebe26cb7968e9a5cce3ab05821dfb81e1221ec
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007561"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="cf21d-103">Tipo de recurso timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="cf21d-103">timeZoneBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf21d-104">A representação básica de um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="cf21d-104">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="cf21d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf21d-105">Properties</span></span>
| <span data-ttu-id="cf21d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf21d-106">Property</span></span>     | <span data-ttu-id="cf21d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf21d-107">Type</span></span>   |<span data-ttu-id="cf21d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf21d-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cf21d-109">name</span><span class="sxs-lookup"><span data-stu-id="cf21d-109">name</span></span> | <span data-ttu-id="cf21d-110">string</span><span class="sxs-lookup"><span data-stu-id="cf21d-110">string</span></span> | <span data-ttu-id="cf21d-111">O nome de um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="cf21d-111">The name of a time zone.</span></span> <span data-ttu-id="cf21d-112">Pode ser o nome de um fuso horário padrão como "Hora Padrão do Havaí Aleuta" ou "Fuso Horário Personalizado" para um fuso horário personalizado.</span><span class="sxs-lookup"><span data-stu-id="cf21d-112">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="cf21d-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cf21d-113">JSON representation</span></span>

<span data-ttu-id="cf21d-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cf21d-114">Here is a JSON representation of the resource.</span></span>

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
