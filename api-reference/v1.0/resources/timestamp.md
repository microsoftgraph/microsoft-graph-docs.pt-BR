---
title: tipo de recurso timeStamp
description: Informações de data e hora para um ponto no tempo.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 33dbc9821d2a58763d81249aebe21a9a2c3aee08
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033583"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="b43a0-103">tipo de recurso timeStamp</span><span class="sxs-lookup"><span data-stu-id="b43a0-103">timeStamp resource type</span></span>

<span data-ttu-id="b43a0-104">Informações de data e hora para um ponto no tempo.</span><span class="sxs-lookup"><span data-stu-id="b43a0-104">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b43a0-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b43a0-105">JSON representation</span></span>

<span data-ttu-id="b43a0-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b43a0-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeStamp"
}-->

```json
{
  "date": "String (timestamp)",
  "time": "String (timestamp)",
  "timeZone": "string"
}

```
## <a name="properties"></a><span data-ttu-id="b43a0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b43a0-107">Properties</span></span>
| <span data-ttu-id="b43a0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b43a0-108">Property</span></span>       | <span data-ttu-id="b43a0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b43a0-109">Type</span></span>    |<span data-ttu-id="b43a0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b43a0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b43a0-111">data</span><span class="sxs-lookup"><span data-stu-id="b43a0-111">date</span></span>|<span data-ttu-id="b43a0-112">Data</span><span class="sxs-lookup"><span data-stu-id="b43a0-112">Date</span></span>|<span data-ttu-id="b43a0-113">A parte de data do carimbo de data/hora.</span><span class="sxs-lookup"><span data-stu-id="b43a0-113">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="b43a0-114">time</span><span class="sxs-lookup"><span data-stu-id="b43a0-114">time</span></span>|<span data-ttu-id="b43a0-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b43a0-115">TimeOfDay</span></span>|<span data-ttu-id="b43a0-116">A parte de tempo do carimbo de data/hora.</span><span class="sxs-lookup"><span data-stu-id="b43a0-116">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="b43a0-117">timeZone</span><span class="sxs-lookup"><span data-stu-id="b43a0-117">timeZone</span></span>|<span data-ttu-id="b43a0-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b43a0-118">String</span></span>|<span data-ttu-id="b43a0-119">A parte de fuso horário do carimbo de data/hora, que é uma das 24 áreas de longitudinal do mundo.</span><span class="sxs-lookup"><span data-stu-id="b43a0-119">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
