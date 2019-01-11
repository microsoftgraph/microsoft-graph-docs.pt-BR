---
title: Tipo de recurso timeConstraint
description: Restringe as sugestões de horário para reuniões a certas horas e dias da semana de acordo com a natureza especificada da atividade e intervalos de tempo disponíveis.
localization_priority: Normal
ms.openlocfilehash: 6e3cc56f1495eae60bb84c458caa25c79557e033
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832904"
---
# <a name="timeconstraint-resource-type"></a><span data-ttu-id="fb7f3-103">Tipo de recurso timeConstraint</span><span class="sxs-lookup"><span data-stu-id="fb7f3-103">timeConstraint resource type</span></span>

> <span data-ttu-id="fb7f3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fb7f3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb7f3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fb7f3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fb7f3-106">Restringe as sugestões de horário para reuniões a certas horas e dias da semana de acordo com a natureza especificada da atividade e intervalos de tempo disponíveis.</span><span class="sxs-lookup"><span data-stu-id="fb7f3-106">Restricts meeting time suggestions to certain hours and days of the week according to the specified nature of activity and open time slots.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb7f3-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fb7f3-107">JSON representation</span></span>

<span data-ttu-id="fb7f3-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="fb7f3-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeconstraint"
}-->

```json
{
  "activityDomain": "String",
  "timeslots": [{"@odata.type": "microsoft.graph.timeSlot"}]
}

```
## <a name="properties"></a><span data-ttu-id="fb7f3-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fb7f3-109">Properties</span></span>
| <span data-ttu-id="fb7f3-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fb7f3-110">Property</span></span>     | <span data-ttu-id="fb7f3-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="fb7f3-111">Type</span></span>   |<span data-ttu-id="fb7f3-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="fb7f3-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fb7f3-113">activityDomain</span><span class="sxs-lookup"><span data-stu-id="fb7f3-113">activityDomain</span></span>|<span data-ttu-id="fb7f3-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fb7f3-114">String</span></span>|<span data-ttu-id="fb7f3-p102">A natureza da atividade, opcional. Os valores possíveis são: `work`, `personal`, `unrestricted` ou `unknown`.</span><span class="sxs-lookup"><span data-stu-id="fb7f3-p102">The nature of the activity, optional. Possible values are: `work`, `personal`, `unrestricted`, or `unknown`.</span></span>|
|<span data-ttu-id="fb7f3-117">intervalos de tempo</span><span class="sxs-lookup"><span data-stu-id="fb7f3-117">timeslots</span></span>|<span data-ttu-id="fb7f3-118">Coleção [timeSlot](timeslot.md)</span><span class="sxs-lookup"><span data-stu-id="fb7f3-118">[timeSlot](timeslot.md) collection</span></span>|<span data-ttu-id="fb7f3-119">Uma matriz de períodos de tempo.</span><span class="sxs-lookup"><span data-stu-id="fb7f3-119">An array of time periods.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
