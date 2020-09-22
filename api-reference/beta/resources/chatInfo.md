---
title: tipo de recurso chatInfo
description: Contém informações associadas às reuniões do Microsoft Teams.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e17f949b46626096238745b23b5332ffa69acf3d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064350"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="88179-103">tipo de recurso chatInfo</span><span class="sxs-lookup"><span data-stu-id="88179-103">chatInfo resource type</span></span>

<span data-ttu-id="88179-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88179-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88179-105">Contém informações associadas às reuniões do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="88179-105">Contains information associated with Microsoft Teams meetings.</span></span>

## <a name="properties"></a><span data-ttu-id="88179-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="88179-106">Properties</span></span>

| <span data-ttu-id="88179-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88179-107">Property</span></span>            | <span data-ttu-id="88179-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="88179-108">Type</span></span>    | <span data-ttu-id="88179-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="88179-109">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="88179-110">messageId</span><span class="sxs-lookup"><span data-stu-id="88179-110">messageId</span></span>           | <span data-ttu-id="88179-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88179-111">String</span></span>  | <span data-ttu-id="88179-112">O identificador exclusivo de uma mensagem em um canal do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="88179-112">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="88179-113">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="88179-113">replyChainMessageId</span></span> | <span data-ttu-id="88179-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88179-114">String</span></span>  | <span data-ttu-id="88179-115">A ID da mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="88179-115">The ID of the reply message.</span></span> |
| <span data-ttu-id="88179-116">threadId</span><span class="sxs-lookup"><span data-stu-id="88179-116">threadId</span></span>            | <span data-ttu-id="88179-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="88179-117">String</span></span>  | <span data-ttu-id="88179-118">O identificador exclusivo de um thread no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="88179-118">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="88179-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="88179-119">JSON representation</span></span>

<span data-ttu-id="88179-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="88179-120">The following is a JSON representation of the resource.</span></span>

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


