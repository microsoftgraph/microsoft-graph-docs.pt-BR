---
title: tipo de recurso chatInfo
description: Contém informações associadas às reuniões do Microsoft Teams.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8602301af0de458f07ab5a9c0af00ec8578c3a61
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507730"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="72cd3-103">tipo de recurso chatInfo</span><span class="sxs-lookup"><span data-stu-id="72cd3-103">chatInfo resource type</span></span>

<span data-ttu-id="72cd3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="72cd3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72cd3-105">Contém informações associadas às reuniões do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="72cd3-105">Contains information associated with Microsoft Teams meetings.</span></span>

## <a name="properties"></a><span data-ttu-id="72cd3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="72cd3-106">Properties</span></span>

| <span data-ttu-id="72cd3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72cd3-107">Property</span></span>            | <span data-ttu-id="72cd3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="72cd3-108">Type</span></span>    | <span data-ttu-id="72cd3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="72cd3-109">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="72cd3-110">messageId</span><span class="sxs-lookup"><span data-stu-id="72cd3-110">messageId</span></span>           | <span data-ttu-id="72cd3-111">String</span><span class="sxs-lookup"><span data-stu-id="72cd3-111">String</span></span>  | <span data-ttu-id="72cd3-112">O identificador exclusivo de uma mensagem em um canal do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="72cd3-112">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="72cd3-113">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="72cd3-113">replyChainMessageId</span></span> | <span data-ttu-id="72cd3-114">String</span><span class="sxs-lookup"><span data-stu-id="72cd3-114">String</span></span>  | <span data-ttu-id="72cd3-115">A ID da mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="72cd3-115">The ID of the reply message.</span></span> |
| <span data-ttu-id="72cd3-116">threadId</span><span class="sxs-lookup"><span data-stu-id="72cd3-116">threadId</span></span>            | <span data-ttu-id="72cd3-117">String</span><span class="sxs-lookup"><span data-stu-id="72cd3-117">String</span></span>  | <span data-ttu-id="72cd3-118">O identificador exclusivo de um thread no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="72cd3-118">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="72cd3-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="72cd3-119">JSON representation</span></span>

<span data-ttu-id="72cd3-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="72cd3-120">The following is a JSON representation of the resource.</span></span>

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
