---
title: Tipo de recurso locationConstraint
description: As condições indicadas por um cliente para o local de uma reunião.
localization_priority: Normal
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c2646e361e81b5d9ec0c45e3bcfe5f867c5ebe97
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807763"
---
# <a name="locationconstraint-resource-type"></a><span data-ttu-id="430fe-103">Tipo de recurso locationConstraint</span><span class="sxs-lookup"><span data-stu-id="430fe-103">locationConstraint resource type</span></span>

<span data-ttu-id="430fe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="430fe-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="430fe-105">As condições indicadas por um cliente para o local de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="430fe-105">The conditions stated by a client for the location of a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="430fe-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="430fe-106">JSON representation</span></span>

<span data-ttu-id="430fe-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="430fe-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locationConstraint"
}-->

```json
{
  "isRequired": true,
  "locations": [{"@odata.type": "microsoft.graph.locationConstraintItem"}],
  "suggestLocation": true
}

```
## <a name="properties"></a><span data-ttu-id="430fe-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="430fe-108">Properties</span></span>
| <span data-ttu-id="430fe-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="430fe-109">Property</span></span>     | <span data-ttu-id="430fe-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="430fe-110">Type</span></span>   |<span data-ttu-id="430fe-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="430fe-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="430fe-112">isRequired</span><span class="sxs-lookup"><span data-stu-id="430fe-112">isRequired</span></span>|<span data-ttu-id="430fe-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="430fe-113">Boolean</span></span>|<span data-ttu-id="430fe-p101">O cliente solicita o serviço para incluir na resposta um local para a reunião. Se isso é verdadeiro e todos os recursos estão ocupados, [findMeetingTimes](../api/user-findmeetingtimes.md) não retorna nenhuma sugestão de horário para a reunião. Se isso é verdadeiro e todos os recursos estão ocupados, **findMeetingTimes** continuará procurando horários para a reunião sem local.</span><span class="sxs-lookup"><span data-stu-id="430fe-p101">The client requests the service to include in the response a meeting location for the meeting. If this is true and all the resources are busy, [findMeetingTimes](../api/user-findmeetingtimes.md) will not return any meeting time suggestions. If this is false and all the resources are busy, **findMeetingTimes** would still look for meeting times without locations.</span></span> |
|<span data-ttu-id="430fe-117">locations</span><span class="sxs-lookup"><span data-stu-id="430fe-117">locations</span></span>|<span data-ttu-id="430fe-118">Coleção [locationConstraintItem](locationconstraintitem.md)</span><span class="sxs-lookup"><span data-stu-id="430fe-118">[locationConstraintItem](locationconstraintitem.md) collection</span></span>|<span data-ttu-id="430fe-119">Informações de restrição de um ou mais locais que o cliente solicita para a reunião.</span><span class="sxs-lookup"><span data-stu-id="430fe-119">Constraint information for one or more locations that the client requests for the meeting.</span></span>|
|<span data-ttu-id="430fe-120">suggestLocation</span><span class="sxs-lookup"><span data-stu-id="430fe-120">suggestLocation</span></span>|<span data-ttu-id="430fe-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="430fe-121">Boolean</span></span>|<span data-ttu-id="430fe-122">O cliente solicita o serviço para sugerir um ou mais locais para a reunião.</span><span class="sxs-lookup"><span data-stu-id="430fe-122">The client requests the service to suggest one or more meeting locations.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
