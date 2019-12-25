---
title: tipo de recurso inviteParticipantsOperation
description: Representa o status de uma operação de convite de participante de execução longa, disparada por uma chamada para a API participante-INVITE.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d0198ae992dc3e741c2962ed4e2c9534f5a76757
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865658"
---
# <a name="inviteparticipantsoperation-resource-type"></a><span data-ttu-id="60b2c-103">tipo de recurso inviteParticipantsOperation</span><span class="sxs-lookup"><span data-stu-id="60b2c-103">inviteParticipantsOperation resource type</span></span>

<span data-ttu-id="60b2c-104">Representa o status de uma operação de convite de participante de execução longa, disparada por uma chamada para a API participante-INVITE.</span><span class="sxs-lookup"><span data-stu-id="60b2c-104">Represents the status of a long-running participant invitation operation, triggered by a call to the participant-invite API.</span></span>

## <a name="properties"></a><span data-ttu-id="60b2c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="60b2c-105">Properties</span></span>

| <span data-ttu-id="60b2c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60b2c-106">Property</span></span>                       | <span data-ttu-id="60b2c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="60b2c-107">Type</span></span>                        | <span data-ttu-id="60b2c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="60b2c-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="60b2c-109">clientContext</span><span class="sxs-lookup"><span data-stu-id="60b2c-109">clientContext</span></span>                  | <span data-ttu-id="60b2c-110">String</span><span class="sxs-lookup"><span data-stu-id="60b2c-110">String</span></span>                      | <span data-ttu-id="60b2c-111">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="60b2c-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="60b2c-112">id</span><span class="sxs-lookup"><span data-stu-id="60b2c-112">id</span></span>                             | <span data-ttu-id="60b2c-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="60b2c-113">String</span></span>                      | <span data-ttu-id="60b2c-114">A ID da operação do servidor. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="60b2c-114">The server operation id. Read-only.</span></span>                                                                                              |
| <span data-ttu-id="60b2c-115">participants</span><span class="sxs-lookup"><span data-stu-id="60b2c-115">participants</span></span> | <span data-ttu-id="60b2c-116">conjunto [invitationParticipantInfo](invitationParticipantInfo.md)</span><span class="sxs-lookup"><span data-stu-id="60b2c-116">[invitationParticipantInfo](invitationParticipantInfo.md) collection</span></span> | <span data-ttu-id="60b2c-117">Os participantes a serem convidados.</span><span class="sxs-lookup"><span data-stu-id="60b2c-117">The participants to invite.</span></span> |
| <span data-ttu-id="60b2c-118">resultInfo</span><span class="sxs-lookup"><span data-stu-id="60b2c-118">resultInfo</span></span>                     | [<span data-ttu-id="60b2c-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="60b2c-119">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="60b2c-120">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="60b2c-120">The result information.</span></span>  <span data-ttu-id="60b2c-121">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="60b2c-121">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="60b2c-122">status</span><span class="sxs-lookup"><span data-stu-id="60b2c-122">status</span></span>                         | <span data-ttu-id="60b2c-123">String</span><span class="sxs-lookup"><span data-stu-id="60b2c-123">String</span></span>                      | <span data-ttu-id="60b2c-124">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="60b2c-124">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="60b2c-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="60b2c-125">Read-only.</span></span>                                                  |

## <a name="json-representation"></a><span data-ttu-id="60b2c-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="60b2c-126">JSON representation</span></span>

<span data-ttu-id="60b2c-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="60b2c-127">The following is a JSON representation of the resource.</span></span>

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
