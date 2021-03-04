---
title: Tipo de recurso rejectJoinResponse
description: Contém uma resposta para rejeitar um participante que tenta ingressar na reunião.
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4219a8093c1914d65f3f36ea1a3b700b47af000c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445889"
---
# <a name="rejectjoinresponse-resource-type"></a><span data-ttu-id="b58fd-103">Tipo de recurso rejectJoinResponse</span><span class="sxs-lookup"><span data-stu-id="b58fd-103">rejectJoinResponse resource type</span></span>

<span data-ttu-id="b58fd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b58fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b58fd-105">Contém uma resposta para rejeitar um participante que tenta ingressar na reunião.</span><span class="sxs-lookup"><span data-stu-id="b58fd-105">Contains a response to reject a participant who tries to join the meeting.</span></span>

<span data-ttu-id="b58fd-106">Isso tem o mesmo efeito que rejeitar uma notificação de chamada de entrada de registro de política usando [o método reject-call.](../api/call-reject.md)</span><span class="sxs-lookup"><span data-stu-id="b58fd-106">This has the same effect as rejecting a policy recording incoming call notification using the [reject-call](../api/call-reject.md) method.</span></span> <span data-ttu-id="b58fd-107">O bot continuará a receber uma notificação de participação de um participante para um novo usuário ingressar até que sua capacidade seja atingida.</span><span class="sxs-lookup"><span data-stu-id="b58fd-107">The bot will continue to receive a participant joining notification for a new user joining until its capacity has been reached.</span></span>

## <a name="properties"></a><span data-ttu-id="b58fd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b58fd-108">Properties</span></span>

| <span data-ttu-id="b58fd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b58fd-109">Property</span></span>         | <span data-ttu-id="b58fd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b58fd-110">Type</span></span>                            | <span data-ttu-id="b58fd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b58fd-111">Description</span></span>                                                                                                                                                  |
| :--------------- | :------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="b58fd-112">motivo</span><span class="sxs-lookup"><span data-stu-id="b58fd-112">reason</span></span>           | <span data-ttu-id="b58fd-113">String</span><span class="sxs-lookup"><span data-stu-id="b58fd-113">String</span></span>                          | <span data-ttu-id="b58fd-114">O motivo da rejeição.</span><span class="sxs-lookup"><span data-stu-id="b58fd-114">The rejection reason.</span></span> <span data-ttu-id="b58fd-115">Os valores possíveis são: `None`, `Busy` e `Forbidden`.</span><span class="sxs-lookup"><span data-stu-id="b58fd-115">Possible values are `None`, `Busy`, and `Forbidden`.</span></span>                                                                                     |

## <a name="json-representation"></a><span data-ttu-id="b58fd-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b58fd-116">JSON representation</span></span>

<span data-ttu-id="b58fd-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b58fd-117">The following is a JSON representation of the resource.</span></span>

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
