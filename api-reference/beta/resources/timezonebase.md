---
title: Tipo de recurso timeZoneBase
description: A representação básica de um fuso horário.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 95347a76ff5622f1e93d6e4c61a6ab050c302db9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519684"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="0dcbb-103">Tipo de recurso timeZoneBase</span><span class="sxs-lookup"><span data-stu-id="0dcbb-103">timeZoneBase resource type</span></span>

<span data-ttu-id="0dcbb-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0dcbb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0dcbb-105">A representação básica de um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="0dcbb-105">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="0dcbb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0dcbb-106">Properties</span></span>
| <span data-ttu-id="0dcbb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0dcbb-107">Property</span></span>     | <span data-ttu-id="0dcbb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0dcbb-108">Type</span></span>   |<span data-ttu-id="0dcbb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0dcbb-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0dcbb-110">nome</span><span class="sxs-lookup"><span data-stu-id="0dcbb-110">name</span></span> | <span data-ttu-id="0dcbb-111">string</span><span class="sxs-lookup"><span data-stu-id="0dcbb-111">string</span></span> | <span data-ttu-id="0dcbb-112">O nome de um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="0dcbb-112">The name of a time zone.</span></span> <span data-ttu-id="0dcbb-113">Pode ser o nome de um fuso horário padrão como "Hora Padrão do Havaí Aleuta" ou "Fuso Horário Personalizado" para um fuso horário personalizado.</span><span class="sxs-lookup"><span data-stu-id="0dcbb-113">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="0dcbb-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0dcbb-114">JSON representation</span></span>

<span data-ttu-id="0dcbb-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0dcbb-115">Here is a JSON representation of the resource.</span></span>

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
