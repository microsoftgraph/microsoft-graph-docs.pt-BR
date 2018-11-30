---
title: tipo de recurso da carimbo de hora
description: Data e hora informações para um ponto no tempo.
ms.openlocfilehash: 4f392e880bb165841fd8a9a31b6ed00bf2ba36fb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004162"
---
# <a name="timestamp-resource-type"></a><span data-ttu-id="8741b-103">tipo de recurso da carimbo de hora</span><span class="sxs-lookup"><span data-stu-id="8741b-103">timeStamp resource type</span></span>

<span data-ttu-id="8741b-104">Data e hora informações para um ponto no tempo.</span><span class="sxs-lookup"><span data-stu-id="8741b-104">Date and time information for a point in time.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8741b-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8741b-105">JSON representation</span></span>

<span data-ttu-id="8741b-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="8741b-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="8741b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8741b-107">Properties</span></span>
| <span data-ttu-id="8741b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8741b-108">Property</span></span>       | <span data-ttu-id="8741b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8741b-109">Type</span></span>    |<span data-ttu-id="8741b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8741b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8741b-111">data</span><span class="sxs-lookup"><span data-stu-id="8741b-111">date</span></span>|<span data-ttu-id="8741b-112">Data</span><span class="sxs-lookup"><span data-stu-id="8741b-112">Date</span></span>|<span data-ttu-id="8741b-113">A parte da data do carimbo de hora.</span><span class="sxs-lookup"><span data-stu-id="8741b-113">The date portion of the timestamp.</span></span>|
|<span data-ttu-id="8741b-114">time</span><span class="sxs-lookup"><span data-stu-id="8741b-114">time</span></span>|<span data-ttu-id="8741b-115">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="8741b-115">TimeOfDay</span></span>|<span data-ttu-id="8741b-116">A parte do tempo do carimbo de hora.</span><span class="sxs-lookup"><span data-stu-id="8741b-116">The time portion of the timestamp.</span></span>|
|<span data-ttu-id="8741b-117">timeZone</span><span class="sxs-lookup"><span data-stu-id="8741b-117">timeZone</span></span>|<span data-ttu-id="8741b-118">String</span><span class="sxs-lookup"><span data-stu-id="8741b-118">String</span></span>|<span data-ttu-id="8741b-119">A porção de fuso horário da carimbo de hora, o que é uma das áreas longitudinal 24 no mundo.</span><span class="sxs-lookup"><span data-stu-id="8741b-119">The timezone portion of the timestamp, which is one of the 24 longitudinal areas in the world.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->