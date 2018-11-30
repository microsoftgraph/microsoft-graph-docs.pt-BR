---
title: tipo de recurso de meetingParticipants
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 4f91c9198018e903eccff7e8fe07d6668d9fd2c9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040712"
---
# <a name="meetingparticipants-resource-type"></a><span data-ttu-id="05866-103">tipo de recurso de meetingParticipants</span><span class="sxs-lookup"><span data-stu-id="05866-103">meetingParticipants resource type</span></span>

> <span data-ttu-id="05866-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="05866-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05866-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="05866-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="05866-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="05866-106">Properties</span></span>

| <span data-ttu-id="05866-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="05866-107">Property</span></span>       | <span data-ttu-id="05866-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="05866-108">Type</span></span>    | <span data-ttu-id="05866-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="05866-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="05866-110">attendees</span><span class="sxs-lookup"><span data-stu-id="05866-110">attendees</span></span> | <span data-ttu-id="05866-111">coleção [meetingParticipantInfo](meetingparticipantinfo.md)</span><span class="sxs-lookup"><span data-stu-id="05866-111">[meetingParticipantInfo](meetingparticipantinfo.md) collection</span></span> |  |
| <span data-ttu-id="05866-112">organizer</span><span class="sxs-lookup"><span data-stu-id="05866-112">organizer</span></span> | [<span data-ttu-id="05866-113">meetingParticipantInfo</span><span class="sxs-lookup"><span data-stu-id="05866-113">meetingParticipantInfo</span></span>](meetingparticipantinfo.md) |  |

## <a name="json-representation"></a><span data-ttu-id="05866-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="05866-114">JSON representation</span></span>

<span data-ttu-id="05866-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="05866-115">The following is a JSON representation of the resource.</span></span>

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
