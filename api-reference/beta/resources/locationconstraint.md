---
title: Tipo de recurso locationConstraint
description: As condições indicadas por um cliente para o local de uma reunião.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f79f6243d996193aacee66c8955ce49c8b779482
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073577"
---
# <a name="locationconstraint-resource-type"></a><span data-ttu-id="bbbdc-103">Tipo de recurso locationConstraint</span><span class="sxs-lookup"><span data-stu-id="bbbdc-103">locationConstraint resource type</span></span>

<span data-ttu-id="bbbdc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbbdc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bbbdc-105">As condições indicadas por um cliente para o local de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="bbbdc-105">The conditions stated by a client for the location of a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bbbdc-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bbbdc-106">JSON representation</span></span>

<span data-ttu-id="bbbdc-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="bbbdc-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="bbbdc-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bbbdc-108">Properties</span></span>
| <span data-ttu-id="bbbdc-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bbbdc-109">Property</span></span>     | <span data-ttu-id="bbbdc-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbbdc-110">Type</span></span>   |<span data-ttu-id="bbbdc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbbdc-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bbbdc-112">isRequired</span><span class="sxs-lookup"><span data-stu-id="bbbdc-112">isRequired</span></span>|<span data-ttu-id="bbbdc-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="bbbdc-113">Boolean</span></span>|<span data-ttu-id="bbbdc-p101">O cliente solicita o serviço para incluir na resposta um local para a reunião. Se isso é verdadeiro e todos os recursos estão ocupados, [findMeetingTimes](../api/user-findmeetingtimes.md) não retorna nenhuma sugestão de horário para a reunião. Se isso é verdadeiro e todos os recursos estão ocupados, **findMeetingTimes** continuará procurando horários para a reunião sem local.</span><span class="sxs-lookup"><span data-stu-id="bbbdc-p101">The client requests the service to include in the response a meeting location for the meeting. If this is true and all the resources are busy, [findMeetingTimes](../api/user-findmeetingtimes.md) will not return any meeting time suggestions. If this is false and all the resources are busy, **findMeetingTimes** would still look for meeting times without locations.</span></span> |
|<span data-ttu-id="bbbdc-117">locations</span><span class="sxs-lookup"><span data-stu-id="bbbdc-117">locations</span></span>|<span data-ttu-id="bbbdc-118">Coleção [locationConstraintItem](locationconstraintitem.md)</span><span class="sxs-lookup"><span data-stu-id="bbbdc-118">[locationConstraintItem](locationconstraintitem.md) collection</span></span>|<span data-ttu-id="bbbdc-119">Informações de restrição de um ou mais locais que o cliente solicita para a reunião.</span><span class="sxs-lookup"><span data-stu-id="bbbdc-119">Constraint information for one or more locations that the client requests for the meeting.</span></span>|
|<span data-ttu-id="bbbdc-120">suggestLocation</span><span class="sxs-lookup"><span data-stu-id="bbbdc-120">suggestLocation</span></span>|<span data-ttu-id="bbbdc-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="bbbdc-121">Boolean</span></span>|<span data-ttu-id="bbbdc-122">O cliente solicita o serviço para sugerir um ou mais locais para a reunião.</span><span class="sxs-lookup"><span data-stu-id="bbbdc-122">The client requests the service to suggest one or more meeting locations.</span></span>|

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


