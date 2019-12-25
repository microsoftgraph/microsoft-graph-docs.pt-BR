---
title: tipo de recurso chatInfo
description: Informações sobre uma mensagem no Microsoft Teams.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b7cd56e21997daf4b88f25acc570f5c062959fa2
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871001"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="44f4a-103">tipo de recurso chatInfo</span><span class="sxs-lookup"><span data-stu-id="44f4a-103">chatInfo resource type</span></span>

<span data-ttu-id="44f4a-104">Ele contém informações associadas às reuniões do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="44f4a-104">This contains information associated with Microsoft Teams meetings.</span></span>

## <a name="properties"></a><span data-ttu-id="44f4a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="44f4a-105">Properties</span></span>

| <span data-ttu-id="44f4a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44f4a-106">Property</span></span>            | <span data-ttu-id="44f4a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="44f4a-107">Type</span></span>    | <span data-ttu-id="44f4a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="44f4a-108">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="44f4a-109">messageId</span><span class="sxs-lookup"><span data-stu-id="44f4a-109">messageId</span></span>           | <span data-ttu-id="44f4a-110">String</span><span class="sxs-lookup"><span data-stu-id="44f4a-110">String</span></span>  | <span data-ttu-id="44f4a-111">O identificador exclusivo de uma mensagem em um canal do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="44f4a-111">The unique identifier of a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="44f4a-112">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="44f4a-112">replyChainMessageId</span></span> | <span data-ttu-id="44f4a-113">String</span><span class="sxs-lookup"><span data-stu-id="44f4a-113">String</span></span>  | <span data-ttu-id="44f4a-114">A ID da mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="44f4a-114">The ID of the reply message.</span></span> |
| <span data-ttu-id="44f4a-115">threadId</span><span class="sxs-lookup"><span data-stu-id="44f4a-115">threadId</span></span>            | <span data-ttu-id="44f4a-116">String</span><span class="sxs-lookup"><span data-stu-id="44f4a-116">String</span></span>  | <span data-ttu-id="44f4a-117">O identificador exclusivo de um thread no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="44f4a-117">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="44f4a-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="44f4a-118">JSON representation</span></span>

<span data-ttu-id="44f4a-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="44f4a-119">The following is a JSON representation of the resource.</span></span>

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
