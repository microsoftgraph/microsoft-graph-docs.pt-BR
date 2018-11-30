---
title: tipo de recurso de chatInfo
description: Informações sobre uma mensagem em Teams da Microsoft.
ms.openlocfilehash: d7e90cf2cdf5180f6483675d919b4e635a1cd5fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033142"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="17905-103">tipo de recurso de chatInfo</span><span class="sxs-lookup"><span data-stu-id="17905-103">chatInfo resource type</span></span>

> <span data-ttu-id="17905-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="17905-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17905-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="17905-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="17905-106">Informações sobre uma mensagem em Teams da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="17905-106">Information about a message in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="17905-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="17905-107">Properties</span></span>

| <span data-ttu-id="17905-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17905-108">Property</span></span>            | <span data-ttu-id="17905-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="17905-109">Type</span></span>    | <span data-ttu-id="17905-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="17905-110">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="17905-111">messageId</span><span class="sxs-lookup"><span data-stu-id="17905-111">messageId</span></span>           | <span data-ttu-id="17905-112">String</span><span class="sxs-lookup"><span data-stu-id="17905-112">String</span></span>  | <span data-ttu-id="17905-113">O identificador exclusivo para uma mensagem em um canal de Teams da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="17905-113">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="17905-114">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="17905-114">replyChainMessageId</span></span> | <span data-ttu-id="17905-115">String</span><span class="sxs-lookup"><span data-stu-id="17905-115">String</span></span>  | <span data-ttu-id="17905-116">A ID da mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="17905-116">The ID of the reply message.</span></span> |
| <span data-ttu-id="17905-117">threadId</span><span class="sxs-lookup"><span data-stu-id="17905-117">threadId</span></span>            | <span data-ttu-id="17905-118">String</span><span class="sxs-lookup"><span data-stu-id="17905-118">String</span></span>  | <span data-ttu-id="17905-119">O identificador exclusivo de um segmento no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="17905-119">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="17905-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="17905-120">JSON representation</span></span>

<span data-ttu-id="17905-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="17905-121">The following is a JSON representation of the resource.</span></span>

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
