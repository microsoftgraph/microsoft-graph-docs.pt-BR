---
title: tipo de recurso de meetingParticipants
description: Participantes em uma reunião.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 309c17cd5594a44e029cce4d618d52c0192f1da3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951919"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="022ed-103">tipo de recurso de meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="022ed-103">meetingParticipants resource type</span></span>

> <span data-ttu-id="022ed-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="022ed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="022ed-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="022ed-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="022ed-106">Participantes em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="022ed-106">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="022ed-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="022ed-107">Properties</span></span>

| <span data-ttu-id="022ed-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="022ed-108">Property</span></span>       | <span data-ttu-id="022ed-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="022ed-109">Type</span></span>    | <span data-ttu-id="022ed-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="022ed-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="022ed-111">attendees</span><span class="sxs-lookup"><span data-stu-id="022ed-111">attendees</span></span> | <span data-ttu-id="022ed-112">coleção [meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="022ed-112">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="022ed-113">organizer</span><span class="sxs-lookup"><span data-stu-id="022ed-113">organizer</span></span> | [<span data-ttu-id="022ed-114">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="022ed-114">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |

## <a name="json-representation"></a><span data-ttu-id="022ed-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="022ed-115">JSON representation</span></span>

<span data-ttu-id="022ed-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="022ed-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipants"
}-->
```json
{
  "attendees": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
  "organizer": {"@odata.type": "#microsoft.graph.meetingParticipantInfo"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingParticipants resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
