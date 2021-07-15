---
title: Tipo de recurso participantLeftNotification
description: Contém detalhes sobre o participante baseado em política que deixou a chamada.
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ee2526ceef6aaf377003f6e802093ec103059c06
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430823"
---
# <a name="participantleftnotification-resource-type"></a><span data-ttu-id="a0530-103">Tipo de recurso participantLeftNotification</span><span class="sxs-lookup"><span data-stu-id="a0530-103">participantLeftNotification resource type</span></span>

<span data-ttu-id="a0530-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0530-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a0530-105">Contém detalhes sobre o participante baseado em política que deixou a chamada.</span><span class="sxs-lookup"><span data-stu-id="a0530-105">Contains details about the policy-based participant who has left the call.</span></span>

<span data-ttu-id="a0530-106">No cenário [de](/microsoftteams/teams-recording-policy) gravação baseado em Política, quando um participante gerenciado pela chamada de bot sair da reunião, um será enviado para o bot para notificar o bot com detalhes do evento à esquerda do `participantLeftNotification` participante.</span><span class="sxs-lookup"><span data-stu-id="a0530-106">Under the [Policy-based recording](/microsoftteams/teams-recording-policy) scenario, when a participant who is managed by the bot call has left the meeting, a `participantLeftNotification` will be sent to the bot to notify the bot with details of the participant left event.</span></span>

## <a name="properties"></a><span data-ttu-id="a0530-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0530-107">Properties</span></span>
| <span data-ttu-id="a0530-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0530-108">Property</span></span>       | <span data-ttu-id="a0530-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0530-109">Type</span></span>            | <span data-ttu-id="a0530-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0530-110">Description</span></span>                                                        |
| -------------- | --------------  | -------------------------------------------                        |
| <span data-ttu-id="a0530-111">call</span><span class="sxs-lookup"><span data-stu-id="a0530-111">call</span></span>           | [<span data-ttu-id="a0530-112">call</span><span class="sxs-lookup"><span data-stu-id="a0530-112">call</span></span>](call.md) | <span data-ttu-id="a0530-113">O objeto call que contém detalhes sobre o evento de participação do participante.</span><span class="sxs-lookup"><span data-stu-id="a0530-113">The call object that contains details about the participant joining event.</span></span> |
| <span data-ttu-id="a0530-114">participantId</span><span class="sxs-lookup"><span data-stu-id="a0530-114">participantId</span></span>  | <span data-ttu-id="a0530-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0530-115">String</span></span>          | <span data-ttu-id="a0530-116">ID do participante na política que saiu da reunião.</span><span class="sxs-lookup"><span data-stu-id="a0530-116">ID of the participant under the policy who has left the meeting.</span></span>        |

## <a name="json-representation"></a><span data-ttu-id="a0530-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0530-117">JSON representation</span></span>

<span data-ttu-id="a0530-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a0530-118">The following is a JSON representation of the resource.</span></span>

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
