---
title: tipo de recurso shiftActivity
description: Representa uma atividade em um turno.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 24946630e9bc3ae9ba418f5c322ab212c022d6d1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343068"
---
# <a name="shiftactivity-resource-type"></a><span data-ttu-id="edd5b-103">tipo de recurso shiftActivity</span><span class="sxs-lookup"><span data-stu-id="edd5b-103">shiftActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edd5b-104">Representa uma atividade em um [turno](shift.md).</span><span class="sxs-lookup"><span data-stu-id="edd5b-104">Represents an activity in a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="edd5b-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="edd5b-105">Properties</span></span>
| <span data-ttu-id="edd5b-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="edd5b-106">Property</span></span>                         | <span data-ttu-id="edd5b-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="edd5b-107">Type</span></span>                    | <span data-ttu-id="edd5b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="edd5b-108">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="edd5b-109">isPago</span><span class="sxs-lookup"><span data-stu-id="edd5b-109">isPaid</span></span>               | `bool`                  | <span data-ttu-id="edd5b-110">Indica se o `microsoft.graph.user` deve ser pago para a atividade durante seu `shift`.</span><span class="sxs-lookup"><span data-stu-id="edd5b-110">Indicates whether the `microsoft.graph.user` should be paid for the activity during their `shift`.</span></span> <span data-ttu-id="edd5b-111">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="edd5b-111">Required.</span></span>    |
| <span data-ttu-id="edd5b-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="edd5b-112">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="edd5b-113">A data e a hora de início `shiftActivity`para o.</span><span class="sxs-lookup"><span data-stu-id="edd5b-113">The start date and time for the `shiftActivity`.</span></span> <span data-ttu-id="edd5b-114">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="edd5b-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="edd5b-115">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="edd5b-115">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="edd5b-116">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="edd5b-116">Required.</span></span> |
| <span data-ttu-id="edd5b-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="edd5b-117">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="edd5b-118">A data e a hora de término `shiftActivity`para o.</span><span class="sxs-lookup"><span data-stu-id="edd5b-118">The end date and time for the `shiftActivity`.</span></span> <span data-ttu-id="edd5b-119">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="edd5b-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="edd5b-120">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="edd5b-120">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="edd5b-121">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="edd5b-121">Required.</span></span>    |
| <span data-ttu-id="edd5b-122">código</span><span class="sxs-lookup"><span data-stu-id="edd5b-122">code</span></span>               | `string`                  | <span data-ttu-id="edd5b-123">Código definido pelo cliente para `shiftActivity`o.</span><span class="sxs-lookup"><span data-stu-id="edd5b-123">Customer defined code for the `shiftActivity`.</span></span> <span data-ttu-id="edd5b-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="edd5b-124">Required.</span></span>    |
| <span data-ttu-id="edd5b-125">displayName</span><span class="sxs-lookup"><span data-stu-id="edd5b-125">displayName</span></span>               | `string`                  | <span data-ttu-id="edd5b-126">O nome do `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="edd5b-126">The name of the `shiftActivity`.</span></span> <span data-ttu-id="edd5b-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="edd5b-127">Required.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="edd5b-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="edd5b-128">JSON representation</span></span>

<span data-ttu-id="edd5b-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="edd5b-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftActivity"
}-->
```json
{
  "isPaid": true,
  "startDateTime": "2019-03-11T15:00:00Z",
  "endDateTime": "2019-03-11T15:15:00Z",
  "code": "",
  "displayName": "Lunch"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shiftActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
