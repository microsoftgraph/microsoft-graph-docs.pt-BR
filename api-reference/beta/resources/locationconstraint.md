---
title: Tipo de recurso locationConstraint
description: As condições indicadas por um cliente para o local de uma reunião.
ms.openlocfilehash: d151ea97aa65aabdb759be4cb90b577606c648a5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034846"
---
# <a name="locationconstraint-resource-type"></a><span data-ttu-id="4a3a6-103">Tipo de recurso locationConstraint</span><span class="sxs-lookup"><span data-stu-id="4a3a6-103">locationConstraint resource type</span></span>

> <span data-ttu-id="4a3a6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4a3a6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a3a6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4a3a6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4a3a6-106">As condições indicadas por um cliente para o local de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="4a3a6-106">The conditions stated by a client for the location of a meeting.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a3a6-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a3a6-107">JSON representation</span></span>

<span data-ttu-id="4a3a6-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="4a3a6-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.locationconstraint"
}-->

```json
{
  "isRequired": true,
  "locations": [{"@odata.type": "microsoft.graph.locationConstraintItem"}],
  "suggestLocation": true
}

```
## <a name="properties"></a><span data-ttu-id="4a3a6-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a3a6-109">Properties</span></span>
| <span data-ttu-id="4a3a6-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a3a6-110">Property</span></span>     | <span data-ttu-id="4a3a6-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a3a6-111">Type</span></span>   |<span data-ttu-id="4a3a6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a3a6-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a3a6-113">isRequired</span><span class="sxs-lookup"><span data-stu-id="4a3a6-113">isRequired</span></span>|<span data-ttu-id="4a3a6-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="4a3a6-114">Boolean</span></span>|<span data-ttu-id="4a3a6-p102">O cliente solicita o serviço para incluir na resposta um local para a reunião. Se isso é verdadeiro e todos os recursos estão ocupados, [findMeetingTimes](../api/user-findmeetingtimes.md) não retorna nenhuma sugestão de horário para a reunião. Se isso é verdadeiro e todos os recursos estão ocupados, **findMeetingTimes** continuará procurando horários para a reunião sem local.</span><span class="sxs-lookup"><span data-stu-id="4a3a6-p102">The client requests the service to include in the response a meeting location for the meeting. If this is true and all the resources are busy, [findMeetingTimes](../api/user-findmeetingtimes.md) will not return any meeting time suggestions. If this is false and all the resources are busy, **findMeetingTimes** would still look for meeting times without locations.</span></span> |
|<span data-ttu-id="4a3a6-118">locations</span><span class="sxs-lookup"><span data-stu-id="4a3a6-118">locations</span></span>|<span data-ttu-id="4a3a6-119">Coleção [locationConstraintItem](locationconstraintitem.md)</span><span class="sxs-lookup"><span data-stu-id="4a3a6-119">[locationConstraintItem](locationconstraintitem.md) collection</span></span>|<span data-ttu-id="4a3a6-120">Informações de restrição de um ou mais locais que o cliente solicita para a reunião.</span><span class="sxs-lookup"><span data-stu-id="4a3a6-120">Constraint information for one or more locations that the client requests for the meeting.</span></span>|
|<span data-ttu-id="4a3a6-121">suggestLocation</span><span class="sxs-lookup"><span data-stu-id="4a3a6-121">suggestLocation</span></span>|<span data-ttu-id="4a3a6-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="4a3a6-122">Boolean</span></span>|<span data-ttu-id="4a3a6-123">O cliente solicita o serviço para sugerir um ou mais locais para a reunião.</span><span class="sxs-lookup"><span data-stu-id="4a3a6-123">The client requests the service to suggest one or more meeting locations.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->