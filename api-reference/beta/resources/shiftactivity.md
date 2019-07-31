---
title: tipo de recurso shiftActivity
description: Representa uma atividade em um turno.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 8acfb16235c90cf6067ad5fd6c5d8e82ae239f8d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965072"
---
# <a name="shiftactivity-resource-type"></a><span data-ttu-id="49d2e-103">tipo de recurso shiftActivity</span><span class="sxs-lookup"><span data-stu-id="49d2e-103">shiftActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49d2e-104">Representa uma atividade em um [turno](shift.md).</span><span class="sxs-lookup"><span data-stu-id="49d2e-104">Represents an activity in a [shift](shift.md).</span></span>

## <a name="properties"></a><span data-ttu-id="49d2e-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="49d2e-105">Properties</span></span>
| <span data-ttu-id="49d2e-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="49d2e-106">Property</span></span>                         | <span data-ttu-id="49d2e-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="49d2e-107">Type</span></span>                    | <span data-ttu-id="49d2e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="49d2e-108">Description</span></span>                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| <span data-ttu-id="49d2e-109">ispago</span><span class="sxs-lookup"><span data-stu-id="49d2e-109">isPaid</span></span>               | `bool`                  | <span data-ttu-id="49d2e-110">Indica se o `microsoft.graph.user` deve ser pago para a atividade durante seu `shift`.</span><span class="sxs-lookup"><span data-stu-id="49d2e-110">Indicates whether the `microsoft.graph.user` should be paid for the activity during their `shift`.</span></span> <span data-ttu-id="49d2e-111">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49d2e-111">Required.</span></span>    |
| <span data-ttu-id="49d2e-112">startDateTime</span><span class="sxs-lookup"><span data-stu-id="49d2e-112">startDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="49d2e-113">A data e a hora de início `shiftActivity`para o.</span><span class="sxs-lookup"><span data-stu-id="49d2e-113">The start date and time for the `shiftActivity`.</span></span> <span data-ttu-id="49d2e-114">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="49d2e-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="49d2e-115">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="49d2e-115">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="49d2e-116">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49d2e-116">Required.</span></span> |
| <span data-ttu-id="49d2e-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="49d2e-117">endDateTime</span></span>               | `DateTimeOffset`                  | <span data-ttu-id="49d2e-118">A data e a hora de término `shiftActivity`para o.</span><span class="sxs-lookup"><span data-stu-id="49d2e-118">The end date and time for the `shiftActivity`.</span></span> <span data-ttu-id="49d2e-119">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="49d2e-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="49d2e-120">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'.</span><span class="sxs-lookup"><span data-stu-id="49d2e-120">For example, midnight UTC on Jan 1, 2014 would look like this: '2014-01-01T00:00:00Z'.</span></span> <span data-ttu-id="49d2e-121">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49d2e-121">Required.</span></span>    |
| <span data-ttu-id="49d2e-122">código</span><span class="sxs-lookup"><span data-stu-id="49d2e-122">code</span></span>               | `string`                  | <span data-ttu-id="49d2e-123">Código definido pelo cliente para `shiftActivity`o.</span><span class="sxs-lookup"><span data-stu-id="49d2e-123">Customer defined code for the `shiftActivity`.</span></span> <span data-ttu-id="49d2e-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49d2e-124">Required.</span></span>    |
| <span data-ttu-id="49d2e-125">displayName</span><span class="sxs-lookup"><span data-stu-id="49d2e-125">displayName</span></span>               | `string`                  | <span data-ttu-id="49d2e-126">O nome do `shiftActivity`.</span><span class="sxs-lookup"><span data-stu-id="49d2e-126">The name of the `shiftActivity`.</span></span> <span data-ttu-id="49d2e-127">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="49d2e-127">Required.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="49d2e-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="49d2e-128">JSON representation</span></span>

<span data-ttu-id="49d2e-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="49d2e-129">Here is a JSON representation of the resource.</span></span>

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
