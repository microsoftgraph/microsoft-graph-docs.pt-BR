---
title: tipo de recurso payloadTypes
description: Representa o conteúdo de dados de uma notificação de usuário bruto ou Visual que será entregue e consumida pelo cliente do aplicativo que está recebendo esta notificação.
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: a35d48839e6932274f4257ce475710ea904878c0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521980"
---
# <a name="payloadtypes-resource-type"></a><span data-ttu-id="79f70-103">tipo de recurso payloadTypes</span><span class="sxs-lookup"><span data-stu-id="79f70-103">payloadTypes resource type</span></span>

<span data-ttu-id="79f70-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="79f70-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79f70-105">Esse recurso representa o conteúdo de dados de uma notificação de usuário bruto ou Visual que será entregue e consumido pelo cliente do aplicativo que está recebendo essa notificação.</span><span class="sxs-lookup"><span data-stu-id="79f70-105">This resource represents data content of a raw or visual user notification that will be delivered to and consumed by the app client receiving this notification.</span></span>

## <a name="properties"></a><span data-ttu-id="79f70-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79f70-106">Properties</span></span>

| <span data-ttu-id="79f70-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79f70-107">Property</span></span>     | <span data-ttu-id="79f70-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="79f70-108">Type</span></span>        | <span data-ttu-id="79f70-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="79f70-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="79f70-110">rawContent</span><span class="sxs-lookup"><span data-stu-id="79f70-110">rawContent</span></span>|<span data-ttu-id="79f70-111">String</span><span class="sxs-lookup"><span data-stu-id="79f70-111">String</span></span>|<span data-ttu-id="79f70-112">O conteúdo de notificação de uma notificação de usuário bruto que será entregue e consumido pelo cliente de aplicativo em todas as plataformas suportadas (Windows, iOS, Android ou webpush) recebendo esta notificação.</span><span class="sxs-lookup"><span data-stu-id="79f70-112">The notification content of a raw user notification that will be delivered to and consumed by the app client on all supported platforms (Windows, iOS, Android or WebPush) receiving this notification.</span></span> <span data-ttu-id="79f70-113">Pelo menos um dos payloads. RawContent ou Payload. VisualContent precisa ser válido para uma solicitação de notificação POST.</span><span class="sxs-lookup"><span data-stu-id="79f70-113">At least one of Payload.RawContent or Payload.VisualContent needs to be valid for a POST Notification request.</span></span>|
|<span data-ttu-id="79f70-114">visualContent</span><span class="sxs-lookup"><span data-stu-id="79f70-114">visualContent</span></span>|[<span data-ttu-id="79f70-115">visualproperties</span><span class="sxs-lookup"><span data-stu-id="79f70-115">visualProperties</span></span>](visualproperties.md)|<span data-ttu-id="79f70-116">O conteúdo visual de uma notificação de usuário visual, que será consumida pela plataforma de notificação em cada plataforma suportada (Windows, iOS e Android somente) e renderizada para o usuário.</span><span class="sxs-lookup"><span data-stu-id="79f70-116">The visual content of a visual user notification, which will be consumed by the notification platform on each supported platform (Windows, iOS and Android only) and rendered for the user.</span></span> <span data-ttu-id="79f70-117">Pelo menos um dos payloads. RawContent ou Payload. VisualContent precisa ser válido para uma solicitação de notificação POST.</span><span class="sxs-lookup"><span data-stu-id="79f70-117">At least one of Payload.RawContent or Payload.VisualContent needs to be valid for a POST Notification request.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="79f70-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79f70-118">JSON representation</span></span>

<span data-ttu-id="79f70-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="79f70-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.payloadTypes",
  "baseType": null
}-->

```json
{
  "rawContent": "String",
  "visualContent": {"@odata.type": "microsoft.graph.visualProperties"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "payloadTypes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->