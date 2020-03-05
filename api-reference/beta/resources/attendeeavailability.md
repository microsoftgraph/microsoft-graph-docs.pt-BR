---
title: Tipo de recurso attendeeAvailability
description: A disponibilidade de um participante.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5c01c12f486fd8efeb5a3c9ba3d90776e480bafa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508140"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="2fae8-103">Tipo de recurso attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="2fae8-103">attendeeAvailability resource type</span></span>

<span data-ttu-id="2fae8-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2fae8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fae8-105">A disponibilidade de um participante.</span><span class="sxs-lookup"><span data-stu-id="2fae8-105">The availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2fae8-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2fae8-106">JSON representation</span></span>

<span data-ttu-id="2fae8-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="2fae8-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailability"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeBase"},
  "availability": "String"
}

```
## <a name="properties"></a><span data-ttu-id="2fae8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2fae8-108">Properties</span></span>
| <span data-ttu-id="2fae8-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2fae8-109">Property</span></span>     | <span data-ttu-id="2fae8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fae8-110">Type</span></span>   |<span data-ttu-id="2fae8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fae8-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2fae8-112">attendee</span><span class="sxs-lookup"><span data-stu-id="2fae8-112">attendee</span></span>|[<span data-ttu-id="2fae8-113">attendeeBase</span><span class="sxs-lookup"><span data-stu-id="2fae8-113">attendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="2fae8-114">O endereço de email e o tipo de participante, se é uma pessoa ou um recurso, e se é obrigatório ou opcional se for uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="2fae8-114">The email address and type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="2fae8-115">availability</span><span class="sxs-lookup"><span data-stu-id="2fae8-115">availability</span></span>|<span data-ttu-id="2fae8-116">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="2fae8-116">freeBusyStatus</span></span>| <span data-ttu-id="2fae8-p101">O status de disponibilidade do participante. Os possíveis valores são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="2fae8-p101">The availability status of the attendee. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
