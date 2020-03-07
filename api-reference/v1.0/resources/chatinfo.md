---
title: tipo de recurso chatInfo
description: Informações sobre uma mensagem no Microsoft Teams.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b69905a0e1d8937c582df3373a4e981f8d8405ff
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533076"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="fa2ae-103">tipo de recurso chatInfo</span><span class="sxs-lookup"><span data-stu-id="fa2ae-103">chatInfo resource type</span></span>

<span data-ttu-id="fa2ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa2ae-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fa2ae-105">Ele contém informações associadas às reuniões do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="fa2ae-105">This contains information associated with Microsoft Teams meetings.</span></span>

## <a name="properties"></a><span data-ttu-id="fa2ae-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fa2ae-106">Properties</span></span>

| <span data-ttu-id="fa2ae-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa2ae-107">Property</span></span>            | <span data-ttu-id="fa2ae-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa2ae-108">Type</span></span>    | <span data-ttu-id="fa2ae-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa2ae-109">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="fa2ae-110">messageId</span><span class="sxs-lookup"><span data-stu-id="fa2ae-110">messageId</span></span>           | <span data-ttu-id="fa2ae-111">String</span><span class="sxs-lookup"><span data-stu-id="fa2ae-111">String</span></span>  | <span data-ttu-id="fa2ae-112">O identificador exclusivo de uma mensagem em um canal do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="fa2ae-112">The unique identifier of a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="fa2ae-113">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="fa2ae-113">replyChainMessageId</span></span> | <span data-ttu-id="fa2ae-114">String</span><span class="sxs-lookup"><span data-stu-id="fa2ae-114">String</span></span>  | <span data-ttu-id="fa2ae-115">A ID da mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="fa2ae-115">The ID of the reply message.</span></span> |
| <span data-ttu-id="fa2ae-116">threadId</span><span class="sxs-lookup"><span data-stu-id="fa2ae-116">threadId</span></span>            | <span data-ttu-id="fa2ae-117">String</span><span class="sxs-lookup"><span data-stu-id="fa2ae-117">String</span></span>  | <span data-ttu-id="fa2ae-118">O identificador exclusivo de um thread no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="fa2ae-118">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fa2ae-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fa2ae-119">JSON representation</span></span>

<span data-ttu-id="fa2ae-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fa2ae-120">The following is a JSON representation of the resource.</span></span>

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
