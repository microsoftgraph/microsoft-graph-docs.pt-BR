---
title: tipo de recurso inviteParticipantsOperation
description: Representa o status de uma operação de convite de participante de execução longa, disparada por uma chamada para a API participante-INVITE.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 26a1b0574473ed540e28b72cd11fd6a10781452b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988993"
---
# <a name="inviteparticipantsoperation-resource-type"></a><span data-ttu-id="daff0-103">tipo de recurso inviteParticipantsOperation</span><span class="sxs-lookup"><span data-stu-id="daff0-103">inviteParticipantsOperation resource type</span></span>

<span data-ttu-id="daff0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="daff0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="daff0-105">Representa o status de uma operação de convite de participante de execução longa, disparada por uma chamada para a API participante-INVITE.</span><span class="sxs-lookup"><span data-stu-id="daff0-105">Represents the status of a long-running participant invitation operation, triggered by a call to the participant-invite API.</span></span>

## <a name="properties"></a><span data-ttu-id="daff0-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="daff0-106">Properties</span></span>

| <span data-ttu-id="daff0-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="daff0-107">Property</span></span>                       | <span data-ttu-id="daff0-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="daff0-108">Type</span></span>                        | <span data-ttu-id="daff0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="daff0-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="daff0-110">clientContext</span><span class="sxs-lookup"><span data-stu-id="daff0-110">clientContext</span></span>                  | <span data-ttu-id="daff0-111">String</span><span class="sxs-lookup"><span data-stu-id="daff0-111">String</span></span>                      | <span data-ttu-id="daff0-112">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="daff0-112">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="daff0-113">id</span><span class="sxs-lookup"><span data-stu-id="daff0-113">id</span></span>                             | <span data-ttu-id="daff0-114">String</span><span class="sxs-lookup"><span data-stu-id="daff0-114">String</span></span>                      | <span data-ttu-id="daff0-115">A ID da operação do servidor. somente leitura.</span><span class="sxs-lookup"><span data-stu-id="daff0-115">The server operation id. Read-only.</span></span>                                                                                              |
| <span data-ttu-id="daff0-116">participants</span><span class="sxs-lookup"><span data-stu-id="daff0-116">participants</span></span> | <span data-ttu-id="daff0-117">conjunto [invitationParticipantInfo](invitationParticipantInfo.md)</span><span class="sxs-lookup"><span data-stu-id="daff0-117">[invitationParticipantInfo](invitationParticipantInfo.md) collection</span></span> | <span data-ttu-id="daff0-118">Os participantes a serem convidados.</span><span class="sxs-lookup"><span data-stu-id="daff0-118">The participants to invite.</span></span> |
| <span data-ttu-id="daff0-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="daff0-119">resultInfo</span></span>                     | [<span data-ttu-id="daff0-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="daff0-120">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="daff0-121">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="daff0-121">The result information.</span></span>  <span data-ttu-id="daff0-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="daff0-122">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="daff0-123">status</span><span class="sxs-lookup"><span data-stu-id="daff0-123">status</span></span>                         | <span data-ttu-id="daff0-124">String</span><span class="sxs-lookup"><span data-stu-id="daff0-124">String</span></span>                      | <span data-ttu-id="daff0-125">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="daff0-125">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="daff0-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="daff0-126">Read-only.</span></span>                                                  |

## <a name="json-representation"></a><span data-ttu-id="daff0-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="daff0-127">JSON representation</span></span>

<span data-ttu-id="daff0-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="daff0-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "participants": [{"@odata.type": "#microsoft.graph.invitationParticipantInfo"}],
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inviteParticipantsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->


