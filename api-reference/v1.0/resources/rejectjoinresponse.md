---
title: Tipo de recurso rejectJoinResponse
description: Contém uma resposta para rejeitar um participante que tenta ingressar na reunião.
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c917b2c5ba0ed273af1c8e89c78b07a80d6c45fc
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2021
ms.locfileid: "53428854"
---
# <a name="rejectjoinresponse-resource-type"></a><span data-ttu-id="ea1f4-103">Tipo de recurso rejectJoinResponse</span><span class="sxs-lookup"><span data-stu-id="ea1f4-103">rejectJoinResponse resource type</span></span>

<span data-ttu-id="ea1f4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea1f4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ea1f4-105">Contém uma resposta para rejeitar um participante que tenta ingressar na reunião.</span><span class="sxs-lookup"><span data-stu-id="ea1f4-105">Contains a response to reject a participant who tries to join the meeting.</span></span>

<span data-ttu-id="ea1f4-106">Isso tem o mesmo efeito que rejeitar uma notificação de chamada de entrada de registro de política usando [o método reject-call.](../api/call-reject.md)</span><span class="sxs-lookup"><span data-stu-id="ea1f4-106">This has the same effect as rejecting a policy recording incoming call notification using the [reject-call](../api/call-reject.md) method.</span></span> <span data-ttu-id="ea1f4-107">O bot continuará a receber uma notificação de participação de um participante para um novo usuário ingressar até que sua capacidade seja atingida.</span><span class="sxs-lookup"><span data-stu-id="ea1f4-107">The bot will continue to receive a participant joining notification for a new user joining until its capacity has been reached.</span></span>

## <a name="properties"></a><span data-ttu-id="ea1f4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea1f4-108">Properties</span></span>

| <span data-ttu-id="ea1f4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea1f4-109">Property</span></span>         | <span data-ttu-id="ea1f4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea1f4-110">Type</span></span>                            | <span data-ttu-id="ea1f4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea1f4-111">Description</span></span>                                                                                                                                                  |
| :--------------- | :------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="ea1f4-112">motivo</span><span class="sxs-lookup"><span data-stu-id="ea1f4-112">reason</span></span>           | <span data-ttu-id="ea1f4-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea1f4-113">String</span></span>                          | <span data-ttu-id="ea1f4-114">O motivo da rejeição.</span><span class="sxs-lookup"><span data-stu-id="ea1f4-114">The rejection reason.</span></span> <span data-ttu-id="ea1f4-115">Os valores possíveis são: `None`, `Busy` e `Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="ea1f4-115">Possible values are `None`, `Busy`, and `Forbidden`.</span></span>                                                                                     |

## <a name="json-representation"></a><span data-ttu-id="ea1f4-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea1f4-116">JSON representation</span></span>

<span data-ttu-id="ea1f4-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea1f4-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.rejectJoinResponse"
}-->
```json
{
  "reason": "None | Busy | Forbidden" 
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "rejectJoinResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
