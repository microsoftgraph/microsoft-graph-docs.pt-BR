---
title: tipo de recurso shiftItem
description: Um shiftItem representa uma versão do turno.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7ff829ca0f43124404b4b99b048c9919368b6009
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657704"
---
# <a name="shiftitem-resource-type"></a><span data-ttu-id="3ccc6-103">tipo de recurso shiftItem</span><span class="sxs-lookup"><span data-stu-id="3ccc6-103">shiftItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ccc6-104">Representa uma versão de um [turno](shift.md).</span><span class="sxs-lookup"><span data-stu-id="3ccc6-104">Represents a version of a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3ccc6-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3ccc6-105">Properties</span></span>
| <span data-ttu-id="3ccc6-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ccc6-106">Property</span></span>                         | <span data-ttu-id="3ccc6-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ccc6-107">Type</span></span>                    | <span data-ttu-id="3ccc6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ccc6-108">Description</span></span>                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="3ccc6-109">notes</span><span class="sxs-lookup"><span data-stu-id="3ccc6-109">notes</span></span>               | `string`                  | <span data-ttu-id="3ccc6-110">As notas para o `shiftItem`.</span><span class="sxs-lookup"><span data-stu-id="3ccc6-110">The notes for the `shiftItem`.</span></span>      |
| <span data-ttu-id="3ccc6-111">displayName</span><span class="sxs-lookup"><span data-stu-id="3ccc6-111">displayName</span></span>               | `string`                  | <span data-ttu-id="3ccc6-112">O nome do `shiftItem`.</span><span class="sxs-lookup"><span data-stu-id="3ccc6-112">The name of the `shiftItem`.</span></span> |
| <span data-ttu-id="3ccc6-113">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3ccc6-113">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="3ccc6-114">A data e a hora de início `shiftItem`para o.</span><span class="sxs-lookup"><span data-stu-id="3ccc6-114">The start date and time for the `shiftItem`.</span></span> <span data-ttu-id="3ccc6-115">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="3ccc6-115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3ccc6-116">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria a seguinte aparência: ' 2014-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="3ccc6-116">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="3ccc6-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ccc6-117">Required.</span></span> |
| <span data-ttu-id="3ccc6-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="3ccc6-118">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="3ccc6-119">A data e a hora de término `shiftItem`para o.</span><span class="sxs-lookup"><span data-stu-id="3ccc6-119">The end date and time for the `shiftItem`.</span></span> <span data-ttu-id="3ccc6-120">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ccc6-120">Required.</span></span> <span data-ttu-id="3ccc6-121">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="3ccc6-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3ccc6-122">Por exemplo, meia-noite UTC em 1º de janeiro de 2014 teria a seguinte aparência: ' 2014-01-01T00:00:00Z '.</span><span class="sxs-lookup"><span data-stu-id="3ccc6-122">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> |
| <span data-ttu-id="3ccc6-123">tema</span><span class="sxs-lookup"><span data-stu-id="3ccc6-123">theme</span></span> | `enum`   |    |  |  | <span data-ttu-id="3ccc6-124">Cores suPortadas: branco; azuis natureza roxa Rosa amarelo acinzentada darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span><span class="sxs-lookup"><span data-stu-id="3ccc6-124">Supported colors: white; blue; green; purple; pink; yellow; gray; darkBlue; darkGreen; darkPurple; darkPink; darkYellow.</span></span> |
| <span data-ttu-id="3ccc6-125">activities</span><span class="sxs-lookup"><span data-stu-id="3ccc6-125">activities</span></span>    | `collection([shiftActivity](shiftactivity.md))`    | <span data-ttu-id="3ccc6-126">Uma parte incremental de um turno que pode abranger detalhes de quando e onde um funcionário está durante o turno.</span><span class="sxs-lookup"><span data-stu-id="3ccc6-126">An incremental part of a shift which can cover details of when and where an employee is during their shift.</span></span> <span data-ttu-id="3ccc6-127">Por exemplo, uma atribuição ou uma quebra ou almoço agendado.</span><span class="sxs-lookup"><span data-stu-id="3ccc6-127">For example, an assignment or a scheduled break or lunch.</span></span> <span data-ttu-id="3ccc6-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ccc6-128">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3ccc6-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3ccc6-129">JSON representation</span></span>

<span data-ttu-id="3ccc6-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3ccc6-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftItem"
}-->
```json
{
  "displayName": "Day shift",
  "notes": "Please do inventory as part of your shift.",
  "startDateTime": "2019-03-11T15:00:00Z",
  "endDateTime": "2019-03-12T00:00:00Z",
  "theme": "blue",
  "activities": [
    {
      "isPaid": true,
      "startDateTime": "2019-03-11T15:00:00Z",
      "endDateTime": "2019-03-11T15:15:00Z",
      "code": "",
      "displayName": "Lunch"
    }
  ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shiftItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/shiftitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
