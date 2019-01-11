---
title: Tipo de recurso locationConstraint
description: As condições indicadas por um cliente para o local de uma reunião.
localization_priority: Normal
ms.openlocfilehash: 2f6d4951eb8654f2100b17ef35d150023dafbc93
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887917"
---
# <a name="locationconstraint-resource-type"></a><span data-ttu-id="f8405-103">Tipo de recurso locationConstraint</span><span class="sxs-lookup"><span data-stu-id="f8405-103">locationConstraint resource type</span></span>

<span data-ttu-id="f8405-104">As condições indicadas por um cliente para o local de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="f8405-104">The conditions stated by a client for the location of a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8405-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f8405-105">JSON representation</span></span>

<span data-ttu-id="f8405-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f8405-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="f8405-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f8405-107">Properties</span></span>
| <span data-ttu-id="f8405-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8405-108">Property</span></span>     | <span data-ttu-id="f8405-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8405-109">Type</span></span>   |<span data-ttu-id="f8405-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8405-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8405-111">isRequired</span><span class="sxs-lookup"><span data-stu-id="f8405-111">isRequired</span></span>|<span data-ttu-id="f8405-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="f8405-112">Boolean</span></span>|<span data-ttu-id="f8405-p101">O cliente solicita o serviço para incluir na resposta um local para a reunião. Se isso é verdadeiro e todos os recursos estão ocupados, [findMeetingTimes](../api/user-findmeetingtimes.md) não retorna nenhuma sugestão de horário para a reunião. Se isso é verdadeiro e todos os recursos estão ocupados, **findMeetingTimes** continuará procurando horários para a reunião sem local.</span><span class="sxs-lookup"><span data-stu-id="f8405-p101">The client requests the service to include in the response a meeting location for the meeting. If this is true and all the resources are busy, [findMeetingTimes](../api/user-findmeetingtimes.md) will not return any meeting time suggestions. If this is false and all the resources are busy, **findMeetingTimes** would still look for meeting times without locations.</span></span> |
|<span data-ttu-id="f8405-116">locations</span><span class="sxs-lookup"><span data-stu-id="f8405-116">locations</span></span>|<span data-ttu-id="f8405-117">Coleção [locationConstraintItem](locationconstraintitem.md)</span><span class="sxs-lookup"><span data-stu-id="f8405-117">[locationConstraintItem](locationconstraintitem.md) collection</span></span>|<span data-ttu-id="f8405-118">Informações de restrição de um ou mais locais que o cliente solicita para a reunião.</span><span class="sxs-lookup"><span data-stu-id="f8405-118">Constraint information for one or more locations that the client requests for the meeting.</span></span>|
|<span data-ttu-id="f8405-119">suggestLocation</span><span class="sxs-lookup"><span data-stu-id="f8405-119">suggestLocation</span></span>|<span data-ttu-id="f8405-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="f8405-120">Boolean</span></span>|<span data-ttu-id="f8405-121">O cliente solicita o serviço para sugerir um ou mais locais para a reunião.</span><span class="sxs-lookup"><span data-stu-id="f8405-121">The client requests the service to suggest one or more meeting locations.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
