---
title: Tipo de recurso locationConstraint
description: As condições indicadas por um cliente para o local de uma reunião.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: b8dffaed7d647c189548261623f1bde4df693fd2
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472039"
---
# <a name="locationconstraint-resource-type"></a><span data-ttu-id="f53fb-103">Tipo de recurso locationConstraint</span><span class="sxs-lookup"><span data-stu-id="f53fb-103">locationConstraint resource type</span></span>

<span data-ttu-id="f53fb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f53fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f53fb-105">As condições indicadas por um cliente para o local de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="f53fb-105">The conditions stated by a client for the location of a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f53fb-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f53fb-106">JSON representation</span></span>

<span data-ttu-id="f53fb-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f53fb-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="f53fb-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f53fb-108">Properties</span></span>
| <span data-ttu-id="f53fb-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f53fb-109">Property</span></span>     | <span data-ttu-id="f53fb-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f53fb-110">Type</span></span>   |<span data-ttu-id="f53fb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f53fb-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f53fb-112">isRequired</span><span class="sxs-lookup"><span data-stu-id="f53fb-112">isRequired</span></span>|<span data-ttu-id="f53fb-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="f53fb-113">Boolean</span></span>|<span data-ttu-id="f53fb-p101">O cliente solicita o serviço para incluir na resposta um local para a reunião. Se isso é verdadeiro e todos os recursos estão ocupados, [findMeetingTimes](../api/user-findmeetingtimes.md) não retorna nenhuma sugestão de horário para a reunião. Se isso é verdadeiro e todos os recursos estão ocupados, **findMeetingTimes** continuará procurando horários para a reunião sem local.</span><span class="sxs-lookup"><span data-stu-id="f53fb-p101">The client requests the service to include in the response a meeting location for the meeting. If this is true and all the resources are busy, [findMeetingTimes](../api/user-findmeetingtimes.md) will not return any meeting time suggestions. If this is false and all the resources are busy, **findMeetingTimes** would still look for meeting times without locations.</span></span> |
|<span data-ttu-id="f53fb-117">locations</span><span class="sxs-lookup"><span data-stu-id="f53fb-117">locations</span></span>|<span data-ttu-id="f53fb-118">Coleção [locationConstraintItem](locationconstraintitem.md)</span><span class="sxs-lookup"><span data-stu-id="f53fb-118">[locationConstraintItem](locationconstraintitem.md) collection</span></span>|<span data-ttu-id="f53fb-119">Informações de restrição de um ou mais locais que o cliente solicita para a reunião.</span><span class="sxs-lookup"><span data-stu-id="f53fb-119">Constraint information for one or more locations that the client requests for the meeting.</span></span>|
|<span data-ttu-id="f53fb-120">suggestLocation</span><span class="sxs-lookup"><span data-stu-id="f53fb-120">suggestLocation</span></span>|<span data-ttu-id="f53fb-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="f53fb-121">Boolean</span></span>|<span data-ttu-id="f53fb-122">O cliente solicita o serviço para sugerir um ou mais locais para a reunião.</span><span class="sxs-lookup"><span data-stu-id="f53fb-122">The client requests the service to suggest one or more meeting locations.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locationConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


