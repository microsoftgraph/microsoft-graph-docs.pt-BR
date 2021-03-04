---
title: Tipo de recurso inviteNewBotResponse
description: Contém uma resposta a uma solicitação para que uma notificação de participação do participante seja enviada novamente como uma notificação de chamada de entrada para o local desejado.
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3811c1b5aa6fe21a361cd371ab0b39e6ea00c7b1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445937"
---
# <a name="invitenewbotresponse-resource-type"></a><span data-ttu-id="29124-103">Tipo de recurso inviteNewBotResponse</span><span class="sxs-lookup"><span data-stu-id="29124-103">inviteNewBotResponse resource type</span></span>

<span data-ttu-id="29124-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29124-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29124-105">Contém uma resposta a uma solicitação para que uma notificação de participação do participante seja enviada novamente como uma notificação de chamada de entrada para o local desejado.</span><span class="sxs-lookup"><span data-stu-id="29124-105">Contains a response to a request to have a participant joining notification sent out again as a incoming call notification to the desired location.</span></span>

## <a name="properties"></a><span data-ttu-id="29124-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="29124-106">Properties</span></span>

| <span data-ttu-id="29124-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29124-107">Property</span></span>         | <span data-ttu-id="29124-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="29124-108">Type</span></span>                            | <span data-ttu-id="29124-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="29124-109">Description</span></span>                                                                                                                                                  |
| :--------------- | :------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="29124-110">inviteUri</span><span class="sxs-lookup"><span data-stu-id="29124-110">inviteUri</span></span>        | <span data-ttu-id="29124-111">String</span><span class="sxs-lookup"><span data-stu-id="29124-111">String</span></span>                          | <span data-ttu-id="29124-112">URI para receber nova notificação de chamada de entrada.</span><span class="sxs-lookup"><span data-stu-id="29124-112">URI to receive new incoming call notification.</span></span>                                                                                                                |

## <a name="json-representation"></a><span data-ttu-id="29124-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="29124-113">JSON representation</span></span>

<span data-ttu-id="29124-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="29124-114">The following is a JSON representation of the resource.</span></span>

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
