---
title: tipo de recurso timeOffItem
description: Representa uma versão do timeOff.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c83a8725a0048a622ed88ec8265be76c30e46cc0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582853"
---
# <a name="timeoffitem-resource-type"></a><span data-ttu-id="da683-103">tipo de recurso timeOffItem</span><span class="sxs-lookup"><span data-stu-id="da683-103">timeOffItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da683-104">Representa uma versão do [timeOff](timeoff.md).</span><span class="sxs-lookup"><span data-stu-id="da683-104">Represents a version of the [timeOff](timeoff.md).</span></span>

## <a name="properties"></a><span data-ttu-id="da683-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da683-105">Properties</span></span>
| <span data-ttu-id="da683-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da683-106">Property</span></span>                         | <span data-ttu-id="da683-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="da683-107">Type</span></span>                    | <span data-ttu-id="da683-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="da683-108">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="da683-109">timeOffReasonId</span><span class="sxs-lookup"><span data-stu-id="da683-109">timeOffReasonId</span></span>               | `string`                  | <span data-ttu-id="da683-110">ID do `timeOffReason` para isso `timeOffItem`.</span><span class="sxs-lookup"><span data-stu-id="da683-110">ID of the `timeOffReason` for this `timeOffItem`.</span></span> <span data-ttu-id="da683-111">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da683-111">Required.</span></span>     |
| <span data-ttu-id="da683-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="da683-112">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="da683-113">A data e a hora de início `timeOffItem`para o.</span><span class="sxs-lookup"><span data-stu-id="da683-113">The start date and time for the `timeOffItem`.</span></span> <span data-ttu-id="da683-114">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da683-114">Required.</span></span> <span data-ttu-id="da683-115">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="da683-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="da683-116">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="da683-116">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="da683-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="da683-117">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="da683-118">A data e a hora de término `timeOffItem`para o.</span><span class="sxs-lookup"><span data-stu-id="da683-118">The end date and time for the `timeOffItem`.</span></span> <span data-ttu-id="da683-119">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da683-119">Required.</span></span> <span data-ttu-id="da683-120">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="da683-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="da683-121">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="da683-121">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="da683-122">tema</span><span class="sxs-lookup"><span data-stu-id="da683-122">theme</span></span> | `enum`   | <span data-ttu-id="da683-123">Cores suPortadas: branco; azuis natureza roxa Rosa amarelo acinzentada darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span><span class="sxs-lookup"><span data-stu-id="da683-123">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="da683-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da683-124">JSON representation</span></span>

<span data-ttu-id="da683-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="da683-125">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffItem"
}-->
```json
{
  "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
  "startDateTime": "2019-03-11T07:00:00Z",
  "endDateTime": "2019-03-12T07:00:00Z",
  "theme": "pink"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOffItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeoffitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
