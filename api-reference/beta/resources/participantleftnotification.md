---
title: Tipo de recurso participantLeftNotification
description: Contém detalhes sobre o participante baseado em política que deixou a chamada.
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2730cd68e8d7ff6c5c238caeaee91fb4a821c836
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445933"
---
# <a name="participantleftnotification-resource-type"></a><span data-ttu-id="f9be5-103">Tipo de recurso participantLeftNotification</span><span class="sxs-lookup"><span data-stu-id="f9be5-103">participantLeftNotification resource type</span></span>

<span data-ttu-id="f9be5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9be5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9be5-105">Contém detalhes sobre o participante baseado em política que deixou a chamada.</span><span class="sxs-lookup"><span data-stu-id="f9be5-105">Contains details about the policy-based participant who has left the call.</span></span>

<span data-ttu-id="f9be5-106">No cenário [de](/microsoftteams/teams-recording-policy) gravação baseado em Política, quando um participante gerenciado pela chamada de bot sair da reunião, um será enviado para o bot para notificar o bot com detalhes do evento à esquerda do `participantLeftNotification` participante.</span><span class="sxs-lookup"><span data-stu-id="f9be5-106">Under the [Policy-based recording](/microsoftteams/teams-recording-policy) scenario, when a participant who is managed by the bot call has left the meeting, a `participantLeftNotification` will be sent to the bot to notify the bot with details of the participant left event.</span></span>

## <a name="properties"></a><span data-ttu-id="f9be5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f9be5-107">Properties</span></span>
| <span data-ttu-id="f9be5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f9be5-108">Property</span></span>       | <span data-ttu-id="f9be5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f9be5-109">Type</span></span>            | <span data-ttu-id="f9be5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9be5-110">Description</span></span>                                                        |
| -------------- | --------------  | -------------------------------------------                        |
| <span data-ttu-id="f9be5-111">call</span><span class="sxs-lookup"><span data-stu-id="f9be5-111">call</span></span>           | [<span data-ttu-id="f9be5-112">call</span><span class="sxs-lookup"><span data-stu-id="f9be5-112">call</span></span>](call.md) | <span data-ttu-id="f9be5-113">O objeto call que contém detalhes sobre o evento de participação do participante.</span><span class="sxs-lookup"><span data-stu-id="f9be5-113">The call object that contains details about the participant joining event.</span></span> |
| <span data-ttu-id="f9be5-114">participantId</span><span class="sxs-lookup"><span data-stu-id="f9be5-114">participantId</span></span>  | <span data-ttu-id="f9be5-115">String</span><span class="sxs-lookup"><span data-stu-id="f9be5-115">String</span></span>          | <span data-ttu-id="f9be5-116">ID do participante na política que saiu da reunião.</span><span class="sxs-lookup"><span data-stu-id="f9be5-116">ID of the participant under the policy who has left the meeting.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="f9be5-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f9be5-117">JSON representation</span></span>

<span data-ttu-id="f9be5-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f9be5-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.participantLeftNotification"
}-->
```json
{
  "participantId": "String",
  "call": {"@odata.type": "#microsoft.graph.call"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantLeftNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

