---
title: Tipo de recurso attendeeAvailability
description: O tipo e a disponibilidade dos participantes.
localization_priority: Normal
ms.openlocfilehash: a00fe38e678c6a51cd252b823a7d2651e531d20a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820465"
---
# <a name="attendeeavailability-resource-type"></a><span data-ttu-id="4bea5-103">Tipo de recurso attendeeAvailability</span><span class="sxs-lookup"><span data-stu-id="4bea5-103">attendeeAvailability resource type</span></span>

> <span data-ttu-id="4bea5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4bea5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4bea5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4bea5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4bea5-106">O tipo e a disponibilidade dos participantes.</span><span class="sxs-lookup"><span data-stu-id="4bea5-106">The type and availability of an attendee.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4bea5-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4bea5-107">JSON representation</span></span>

<span data-ttu-id="4bea5-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="4bea5-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="4bea5-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4bea5-109">Properties</span></span>
| <span data-ttu-id="4bea5-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4bea5-110">Property</span></span>     | <span data-ttu-id="4bea5-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4bea5-111">Type</span></span>   |<span data-ttu-id="4bea5-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bea5-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4bea5-113">attendee</span><span class="sxs-lookup"><span data-stu-id="4bea5-113">attendee</span></span>|[<span data-ttu-id="4bea5-114">AttendeeBase</span><span class="sxs-lookup"><span data-stu-id="4bea5-114">AttendeeBase</span></span>](attendeebase.md)|<span data-ttu-id="4bea5-115">O tipo de participante, ou seja, se é um recurso ou uma pessoa e, no caso de uma pessoa, se é obrigatório ou opcional.</span><span class="sxs-lookup"><span data-stu-id="4bea5-115">The type of attendee - whether it's a person or a resource, and whether required or optional if it's a person.</span></span>|
|<span data-ttu-id="4bea5-116">availability</span><span class="sxs-lookup"><span data-stu-id="4bea5-116">availability</span></span>|<span data-ttu-id="4bea5-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4bea5-117">String</span></span>| <span data-ttu-id="4bea5-p102">O status de disponibilidade do participante. Os possíveis valores são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="4bea5-p102">The availability status of the attendee. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
