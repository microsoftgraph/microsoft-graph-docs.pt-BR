---
title: Tipo de recurso participantJoiningNotification
description: Contém detalhes sobre o participante baseado em política ingressar em uma chamada.
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3a0067f5632e34a30da7f6f4ec2e8df70995fa88
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445936"
---
# <a name="participantjoiningnotification-resource-type"></a><span data-ttu-id="ff66e-103">Tipo de recurso participantJoiningNotification</span><span class="sxs-lookup"><span data-stu-id="ff66e-103">participantJoiningNotification resource type</span></span>

<span data-ttu-id="ff66e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff66e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff66e-105">Contém detalhes sobre o participante baseado em política ingressar em uma chamada.</span><span class="sxs-lookup"><span data-stu-id="ff66e-105">Contains details about the policy-based participant joining a call.</span></span>

<span data-ttu-id="ff66e-106">No cenário [de](/microsoftteams/teams-recording-policy)registro baseado em política , antes de um participante na política ingressar em uma chamada, um será enviado para o bot associado à política que tem capacidade disponível para lidar com o `participantJoiningNotification` novo participante.</span><span class="sxs-lookup"><span data-stu-id="ff66e-106">Under the [Policy-based recording scenario](/microsoftteams/teams-recording-policy), before a participant under the policy joins a call, a `participantJoiningNotification` will be sent to the bot associated with the policy that has available capacity to handle the new participant.</span></span>

<span data-ttu-id="ff66e-107">Um [participanteJoiningResponse](participantjoiningResponse.md) na carga de resposta é esperado do bot.</span><span class="sxs-lookup"><span data-stu-id="ff66e-107">A [participantJoiningResponse](participantjoiningResponse.md) in the response payload is expected from the bot.</span></span>

## <a name="properties"></a><span data-ttu-id="ff66e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff66e-108">Properties</span></span>
| <span data-ttu-id="ff66e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff66e-109">Property</span></span>       | <span data-ttu-id="ff66e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff66e-110">Type</span></span>            | <span data-ttu-id="ff66e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff66e-111">Description</span></span>                                                        |
| -------------- | --------------  | -------------------------------------------                        |
| <span data-ttu-id="ff66e-112">call</span><span class="sxs-lookup"><span data-stu-id="ff66e-112">call</span></span>           | [<span data-ttu-id="ff66e-113">call</span><span class="sxs-lookup"><span data-stu-id="ff66e-113">call</span></span>](call.md) | <span data-ttu-id="ff66e-114">O objeto call que contém detalhes sobre o evento de participação do participante.</span><span class="sxs-lookup"><span data-stu-id="ff66e-114">The call object that contains details about the participant joining event.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ff66e-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff66e-115">JSON representation</span></span>

<span data-ttu-id="ff66e-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff66e-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.participantJoiningNotification"
}-->
```json
{
  "call": {"@odata.type": "#microsoft.graph.call"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantJoiningNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

