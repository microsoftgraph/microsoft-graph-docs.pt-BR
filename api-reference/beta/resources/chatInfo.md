---
title: tipo de recurso de chatInfo
description: Informações sobre uma mensagem em Teams da Microsoft.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: c2cc0dd288abdab7852017600c4c55b9a40b0aa7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852938"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="c7877-103">tipo de recurso de chatInfo</span><span class="sxs-lookup"><span data-stu-id="c7877-103">chatInfo resource type</span></span>

> <span data-ttu-id="c7877-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c7877-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7877-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c7877-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c7877-106">Informações sobre uma mensagem em Teams da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c7877-106">Information about a message in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="c7877-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c7877-107">Properties</span></span>

| <span data-ttu-id="c7877-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c7877-108">Property</span></span>            | <span data-ttu-id="c7877-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c7877-109">Type</span></span>    | <span data-ttu-id="c7877-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c7877-110">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="c7877-111">messageId</span><span class="sxs-lookup"><span data-stu-id="c7877-111">messageId</span></span>           | <span data-ttu-id="c7877-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7877-112">String</span></span>  | <span data-ttu-id="c7877-113">O identificador exclusivo para uma mensagem em um canal de Teams da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c7877-113">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="c7877-114">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="c7877-114">replyChainMessageId</span></span> | <span data-ttu-id="c7877-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7877-115">String</span></span>  | <span data-ttu-id="c7877-116">A ID da mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="c7877-116">The ID of the reply message.</span></span> |
| <span data-ttu-id="c7877-117">threadId</span><span class="sxs-lookup"><span data-stu-id="c7877-117">threadId</span></span>            | <span data-ttu-id="c7877-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c7877-118">String</span></span>  | <span data-ttu-id="c7877-119">O identificador exclusivo de um segmento no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c7877-119">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c7877-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c7877-120">JSON representation</span></span>

<span data-ttu-id="c7877-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c7877-121">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "chatInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
