---
title: tipo de recurso chatInfo
description: Informações sobre uma mensagem no Microsoft Teams.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1cf5dc67aa4a3db8b495f8942f64e05ba0bbc6a4
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006716"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="ce42f-103">tipo de recurso chatInfo</span><span class="sxs-lookup"><span data-stu-id="ce42f-103">chatInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce42f-104">Informações sobre uma mensagem no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ce42f-104">Information about a message in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="ce42f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ce42f-105">Properties</span></span>

| <span data-ttu-id="ce42f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce42f-106">Property</span></span>            | <span data-ttu-id="ce42f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce42f-107">Type</span></span>    | <span data-ttu-id="ce42f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce42f-108">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="ce42f-109">messageId</span><span class="sxs-lookup"><span data-stu-id="ce42f-109">messageId</span></span>           | <span data-ttu-id="ce42f-110">String</span><span class="sxs-lookup"><span data-stu-id="ce42f-110">String</span></span>  | <span data-ttu-id="ce42f-111">O identificador exclusivo de uma mensagem em um canal do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ce42f-111">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="ce42f-112">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="ce42f-112">replyChainMessageId</span></span> | <span data-ttu-id="ce42f-113">String</span><span class="sxs-lookup"><span data-stu-id="ce42f-113">String</span></span>  | <span data-ttu-id="ce42f-114">A ID da mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="ce42f-114">The ID of the reply message.</span></span> |
| <span data-ttu-id="ce42f-115">threadId</span><span class="sxs-lookup"><span data-stu-id="ce42f-115">threadId</span></span>            | <span data-ttu-id="ce42f-116">String</span><span class="sxs-lookup"><span data-stu-id="ce42f-116">String</span></span>  | <span data-ttu-id="ce42f-117">O identificador exclusivo de um thread no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ce42f-117">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ce42f-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ce42f-118">JSON representation</span></span>

<span data-ttu-id="ce42f-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ce42f-119">The following is a JSON representation of the resource.</span></span>

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
