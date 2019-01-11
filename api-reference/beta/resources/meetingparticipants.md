---
title: tipo de recurso de meetingParticipants
description: Participantes em uma reunião.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: fad06a015429a7264d808b4997c94e90e4799825
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815112"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="f06a6-103">tipo de recurso de meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="f06a6-103">meetingParticipants resource type</span></span>

> <span data-ttu-id="f06a6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f06a6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f06a6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f06a6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f06a6-106">Participantes em uma reunião.</span><span class="sxs-lookup"><span data-stu-id="f06a6-106">Participants in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="f06a6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f06a6-107">Properties</span></span>

| <span data-ttu-id="f06a6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f06a6-108">Property</span></span>       | <span data-ttu-id="f06a6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f06a6-109">Type</span></span>    | <span data-ttu-id="f06a6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f06a6-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f06a6-111">attendees</span><span class="sxs-lookup"><span data-stu-id="f06a6-111">attendees</span></span> | <span data-ttu-id="f06a6-112">coleção [meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="f06a6-112">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="f06a6-113">organizer</span><span class="sxs-lookup"><span data-stu-id="f06a6-113">organizer</span></span> | [<span data-ttu-id="f06a6-114">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="f06a6-114">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |

## <a name="json-representation"></a><span data-ttu-id="f06a6-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f06a6-115">JSON representation</span></span>

<span data-ttu-id="f06a6-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f06a6-116">The following is a JSON representation of the resource.</span></span>

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
