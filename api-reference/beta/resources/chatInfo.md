---
title: tipo de recurso chatInfo
description: Contém informações associadas às reuniões do Microsoft Teams.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cb3806cf28e5557d7b5e4bf0296083e3c595047c
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913146"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="ae819-103">tipo de recurso chatInfo</span><span class="sxs-lookup"><span data-stu-id="ae819-103">chatInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae819-104">Contém informações associadas às reuniões do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ae819-104">Contains information associated with Microsoft Teams meetings.</span></span>

## <a name="properties"></a><span data-ttu-id="ae819-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ae819-105">Properties</span></span>

| <span data-ttu-id="ae819-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae819-106">Property</span></span>            | <span data-ttu-id="ae819-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae819-107">Type</span></span>    | <span data-ttu-id="ae819-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae819-108">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="ae819-109">messageId</span><span class="sxs-lookup"><span data-stu-id="ae819-109">messageId</span></span>           | <span data-ttu-id="ae819-110">String</span><span class="sxs-lookup"><span data-stu-id="ae819-110">String</span></span>  | <span data-ttu-id="ae819-111">O identificador exclusivo de uma mensagem em um canal do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ae819-111">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="ae819-112">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="ae819-112">replyChainMessageId</span></span> | <span data-ttu-id="ae819-113">String</span><span class="sxs-lookup"><span data-stu-id="ae819-113">String</span></span>  | <span data-ttu-id="ae819-114">A ID da mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="ae819-114">The ID of the reply message.</span></span> |
| <span data-ttu-id="ae819-115">threadId</span><span class="sxs-lookup"><span data-stu-id="ae819-115">threadId</span></span>            | <span data-ttu-id="ae819-116">String</span><span class="sxs-lookup"><span data-stu-id="ae819-116">String</span></span>  | <span data-ttu-id="ae819-117">O identificador exclusivo de um thread no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ae819-117">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ae819-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ae819-118">JSON representation</span></span>

<span data-ttu-id="ae819-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ae819-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatInfo"
}-->
```json
{
  "messageId": "String",
  "replyChainMessageId": "String",
  "threadId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chatInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
