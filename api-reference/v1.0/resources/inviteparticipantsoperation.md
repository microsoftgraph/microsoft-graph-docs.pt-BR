---
title: tipo de recurso inviteParticipantsOperation
description: Representa o status de uma operação de convite de participante de execução longa, disparada por uma chamada para a API participante-INVITE.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 54223a5b9e807dc45a9868b3251b8d8b1a0fcd72
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447686"
---
# <a name="inviteparticipantsoperation-resource-type"></a><span data-ttu-id="d7650-103">tipo de recurso inviteParticipantsOperation</span><span class="sxs-lookup"><span data-stu-id="d7650-103">inviteParticipantsOperation resource type</span></span>

<span data-ttu-id="d7650-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d7650-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d7650-105">Representa o status de uma operação de convite de participante de execução longa, disparada por uma chamada para a API participante-INVITE.</span><span class="sxs-lookup"><span data-stu-id="d7650-105">Represents the status of a long-running participant invitation operation, triggered by a call to the participant-invite API.</span></span>

## <a name="properties"></a><span data-ttu-id="d7650-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d7650-106">Properties</span></span>

| <span data-ttu-id="d7650-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7650-107">Property</span></span>                       | <span data-ttu-id="d7650-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7650-108">Type</span></span>                        | <span data-ttu-id="d7650-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7650-109">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d7650-110">clientContext</span><span class="sxs-lookup"><span data-stu-id="d7650-110">clientContext</span></span>                  | <span data-ttu-id="d7650-111">String</span><span class="sxs-lookup"><span data-stu-id="d7650-111">String</span></span>                      | <span data-ttu-id="d7650-112">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="d7650-112">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="d7650-113">id</span><span class="sxs-lookup"><span data-stu-id="d7650-113">id</span></span>                             | <span data-ttu-id="d7650-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d7650-114">String</span></span>                      | <span data-ttu-id="d7650-115">A ID da operação do servidor. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d7650-115">The server operation id. Read-only.</span></span>                                                                                              |
| <span data-ttu-id="d7650-116">participantes</span><span class="sxs-lookup"><span data-stu-id="d7650-116">participants</span></span> | <span data-ttu-id="d7650-117">conjunto [invitationParticipantInfo](invitationParticipantInfo.md)</span><span class="sxs-lookup"><span data-stu-id="d7650-117">[invitationParticipantInfo](invitationParticipantInfo.md) collection</span></span> | <span data-ttu-id="d7650-118">Os participantes a serem convidados.</span><span class="sxs-lookup"><span data-stu-id="d7650-118">The participants to invite.</span></span> |
| <span data-ttu-id="d7650-119">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d7650-119">resultInfo</span></span>                     | [<span data-ttu-id="d7650-120">resultInfo</span><span class="sxs-lookup"><span data-stu-id="d7650-120">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="d7650-121">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="d7650-121">The result information.</span></span>  <span data-ttu-id="d7650-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d7650-122">Read-only.</span></span>                                                                                             |
| <span data-ttu-id="d7650-123">status</span><span class="sxs-lookup"><span data-stu-id="d7650-123">status</span></span>                         | <span data-ttu-id="d7650-124">String</span><span class="sxs-lookup"><span data-stu-id="d7650-124">String</span></span>                      | <span data-ttu-id="d7650-125">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="d7650-125">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="d7650-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="d7650-126">Read-only.</span></span>                                                  |

## <a name="json-representation"></a><span data-ttu-id="d7650-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d7650-127">JSON representation</span></span>

<span data-ttu-id="d7650-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d7650-128">The following is a JSON representation of the resource.</span></span>

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
