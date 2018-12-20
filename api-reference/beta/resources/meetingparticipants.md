---
title: tipo de recurso de meetingParticipants
description: Participantes em uma reunião.
author: VinodRavichandran
ms.openlocfilehash: 7e44863004dab5405251e2effaf2af8c2ae31f67
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380279"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="6ec53-103">tipo de recurso de meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="6ec53-103">meetingParticipants resource type</span></span>

> <span data-ttu-id="6ec53-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6ec53-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ec53-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6ec53-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6ec53-106">Participantes em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="6ec53-106">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="6ec53-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6ec53-107">Properties</span></span>

| <span data-ttu-id="6ec53-108">Propriedade	</span><span class="sxs-lookup"><span data-stu-id="6ec53-108">Property</span></span>       | <span data-ttu-id="6ec53-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ec53-109">Type</span></span>    | <span data-ttu-id="6ec53-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ec53-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6ec53-111">attendees</span><span class="sxs-lookup"><span data-stu-id="6ec53-111">attendees</span></span> | <span data-ttu-id="6ec53-112">coleção [meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="6ec53-112">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="6ec53-113">organizer</span><span class="sxs-lookup"><span data-stu-id="6ec53-113">organizer</span></span> | [<span data-ttu-id="6ec53-114">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="6ec53-114">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |

## <a name="json-representation"></a><span data-ttu-id="6ec53-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6ec53-115">JSON representation</span></span>

<span data-ttu-id="6ec53-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6ec53-116">The following is a JSON representation of the resource.</span></span>

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
