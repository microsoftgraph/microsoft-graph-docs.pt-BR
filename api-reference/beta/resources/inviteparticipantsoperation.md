---
title: tipo de recurso inviteParticipantsOperation
description: Representa o status de uma operação de convite de participante de execução longa, disparada por uma chamada para a API participante-INVITE.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a974bd22ddd9e1ac8c6ab90cdedb9dda9f1a1bb5
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/07/2019
ms.locfileid: "36793017"
---
# <a name="inviteparticipantsoperation-resource-type"></a><span data-ttu-id="87e88-103">tipo de recurso inviteParticipantsOperation</span><span class="sxs-lookup"><span data-stu-id="87e88-103">inviteParticipantsOperation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87e88-104">Representa o status de uma operação de convite de participante de execução longa, disparada por uma chamada para a API participante-INVITE.</span><span class="sxs-lookup"><span data-stu-id="87e88-104">Represents the status of a long-running participant invitation operation, triggered by a call to the participant-invite API.</span></span>

## <a name="properties"></a><span data-ttu-id="87e88-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87e88-105">Properties</span></span>

| <span data-ttu-id="87e88-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87e88-106">Property</span></span>                       | <span data-ttu-id="87e88-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="87e88-107">Type</span></span>                        | <span data-ttu-id="87e88-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="87e88-108">Description</span></span>                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="87e88-109">clientContext</span><span class="sxs-lookup"><span data-stu-id="87e88-109">clientContext</span></span>                  | <span data-ttu-id="87e88-110">String</span><span class="sxs-lookup"><span data-stu-id="87e88-110">String</span></span>                      | <span data-ttu-id="87e88-111">O contexto do cliente.</span><span class="sxs-lookup"><span data-stu-id="87e88-111">The client context.</span></span>                                                                                                                               |
| <span data-ttu-id="87e88-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="87e88-112">createdDateTime</span></span>                | <span data-ttu-id="87e88-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87e88-113">DateTimeOffset</span></span>              | <span data-ttu-id="87e88-114">A hora em que a gravação foi criada.</span><span class="sxs-lookup"><span data-stu-id="87e88-114">The time when the recording was created.</span></span>                                                                                                          |
| <span data-ttu-id="87e88-115">id</span><span class="sxs-lookup"><span data-stu-id="87e88-115">id</span></span>                             | <span data-ttu-id="87e88-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="87e88-116">String</span></span>                      | <span data-ttu-id="87e88-117">A ID da operação do servidor. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="87e88-117">The server operation id. Read-only.</span></span> <span data-ttu-id="87e88-118">Servidor gerado.</span><span class="sxs-lookup"><span data-stu-id="87e88-118">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="87e88-119">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="87e88-119">lastActionDateTime</span></span>             | <span data-ttu-id="87e88-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87e88-120">DateTimeOffset</span></span>              | <span data-ttu-id="87e88-121">A hora da última ação da operação.</span><span class="sxs-lookup"><span data-stu-id="87e88-121">The time of the last action of the operation.</span></span>                                                                                                     |
| <span data-ttu-id="87e88-122">participants</span><span class="sxs-lookup"><span data-stu-id="87e88-122">participants</span></span> | <span data-ttu-id="87e88-123">coleção [invitationParticipantInfo](invitationParticipantInfo.md)</span><span class="sxs-lookup"><span data-stu-id="87e88-123">[invitationParticipantInfo](invitationParticipantInfo.md) collection</span></span> | <span data-ttu-id="87e88-124">Os participantes a serem convidados.</span><span class="sxs-lookup"><span data-stu-id="87e88-124">The participants to invite.</span></span> |
| <span data-ttu-id="87e88-125">resultInfo</span><span class="sxs-lookup"><span data-stu-id="87e88-125">resultInfo</span></span>                     | [<span data-ttu-id="87e88-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="87e88-126">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="87e88-127">As informações de resultado.</span><span class="sxs-lookup"><span data-stu-id="87e88-127">The result information.</span></span>  <span data-ttu-id="87e88-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="87e88-128">Read-only.</span></span> <span data-ttu-id="87e88-129">Servidor gerado.</span><span class="sxs-lookup"><span data-stu-id="87e88-129">Server generated.</span></span>                                                                                             |
| <span data-ttu-id="87e88-130">status</span><span class="sxs-lookup"><span data-stu-id="87e88-130">status</span></span>                         | <span data-ttu-id="87e88-131">String</span><span class="sxs-lookup"><span data-stu-id="87e88-131">String</span></span>                      | <span data-ttu-id="87e88-132">Os valores possíveis são: `notStarted`, `running`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="87e88-132">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="87e88-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="87e88-133">Read-only.</span></span> <span data-ttu-id="87e88-134">Servidor gerado.</span><span class="sxs-lookup"><span data-stu-id="87e88-134">Server generated.</span></span>                                                 |

## <a name="relationships"></a><span data-ttu-id="87e88-135">Relações</span><span class="sxs-lookup"><span data-stu-id="87e88-135">Relationships</span></span>
<span data-ttu-id="87e88-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="87e88-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="87e88-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87e88-137">JSON representation</span></span>

<span data-ttu-id="87e88-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="87e88-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
}-->
```json
{
  "clientContext": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
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
