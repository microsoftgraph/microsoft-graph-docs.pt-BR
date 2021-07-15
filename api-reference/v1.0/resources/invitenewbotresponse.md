---
title: Tipo de recurso inviteNewBotResponse
description: Contém uma resposta a uma solicitação para que uma notificação de participação do participante seja enviada novamente como uma notificação de chamada de entrada para o local desejado.
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 675b7cd1df35b25e3414f36a4dd04e389e05b192
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430183"
---
# <a name="invitenewbotresponse-resource-type"></a><span data-ttu-id="f21c9-103">Tipo de recurso inviteNewBotResponse</span><span class="sxs-lookup"><span data-stu-id="f21c9-103">inviteNewBotResponse resource type</span></span>

<span data-ttu-id="f21c9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f21c9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f21c9-105">Contém uma resposta a uma solicitação para que uma notificação de participação do participante seja enviada novamente como uma notificação de chamada de entrada para o local desejado.</span><span class="sxs-lookup"><span data-stu-id="f21c9-105">Contains a response to a request to have a participant joining notification sent out again as a incoming call notification to the desired location.</span></span>

## <a name="properties"></a><span data-ttu-id="f21c9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f21c9-106">Properties</span></span>

| <span data-ttu-id="f21c9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f21c9-107">Property</span></span>         | <span data-ttu-id="f21c9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f21c9-108">Type</span></span>                            | <span data-ttu-id="f21c9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f21c9-109">Description</span></span>                                                                                                                                                  |
| :--------------- | :------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f21c9-110">inviteUri</span><span class="sxs-lookup"><span data-stu-id="f21c9-110">inviteUri</span></span>        | <span data-ttu-id="f21c9-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f21c9-111">String</span></span>                          | <span data-ttu-id="f21c9-112">URI para receber nova notificação de chamada de entrada.</span><span class="sxs-lookup"><span data-stu-id="f21c9-112">URI to receive new incoming call notification.</span></span>                                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="f21c9-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f21c9-113">JSON representation</span></span>

<span data-ttu-id="f21c9-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f21c9-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.inviteNewBotResponse"
}-->
```json
{
  "inviteUri": "uri" 
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "inviteNewBotResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
