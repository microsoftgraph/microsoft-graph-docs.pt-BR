---
title: tipo de recurso chatInfo
description: Informações sobre uma mensagem no Microsoft Teams.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 552844795d3ba7e8ad4c8a3c3a6dff3c18990bc2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339690"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="ebed8-103">tipo de recurso chatInfo</span><span class="sxs-lookup"><span data-stu-id="ebed8-103">chatInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebed8-104">Informações sobre uma mensagem no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ebed8-104">Information about a message in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="ebed8-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ebed8-105">Properties</span></span>

| <span data-ttu-id="ebed8-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ebed8-106">Property</span></span>            | <span data-ttu-id="ebed8-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebed8-107">Type</span></span>    | <span data-ttu-id="ebed8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebed8-108">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="ebed8-109">messageId</span><span class="sxs-lookup"><span data-stu-id="ebed8-109">messageId</span></span>           | <span data-ttu-id="ebed8-110">String</span><span class="sxs-lookup"><span data-stu-id="ebed8-110">String</span></span>  | <span data-ttu-id="ebed8-111">O identificador exclusivo de uma mensagem em um canal do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ebed8-111">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="ebed8-112">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="ebed8-112">replyChainMessageId</span></span> | <span data-ttu-id="ebed8-113">String</span><span class="sxs-lookup"><span data-stu-id="ebed8-113">String</span></span>  | <span data-ttu-id="ebed8-114">A ID da mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="ebed8-114">The ID of the reply message.</span></span> |
| <span data-ttu-id="ebed8-115">threadId</span><span class="sxs-lookup"><span data-stu-id="ebed8-115">threadId</span></span>            | <span data-ttu-id="ebed8-116">String</span><span class="sxs-lookup"><span data-stu-id="ebed8-116">String</span></span>  | <span data-ttu-id="ebed8-117">O identificador exclusivo de um thread no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ebed8-117">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ebed8-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ebed8-118">JSON representation</span></span>

<span data-ttu-id="ebed8-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ebed8-119">The following is a JSON representation of the resource.</span></span>

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
