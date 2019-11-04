---
title: tipo de recurso payloadTypes
description: Representa o conteúdo de dados de uma notificação de usuário bruto ou Visual que será entregue e consumida pelo cliente do aplicativo que está recebendo esta notificação.
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: 2d740c5b19b363fa2534984bf059cd186b065e89
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939604"
---
# <a name="payloadtypes-resource-type"></a><span data-ttu-id="f5401-103">tipo de recurso payloadTypes</span><span class="sxs-lookup"><span data-stu-id="f5401-103">payloadTypes resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5401-104">Esse recurso representa o conteúdo de dados de uma notificação de usuário bruto ou Visual que será entregue e consumido pelo cliente do aplicativo que está recebendo essa notificação.</span><span class="sxs-lookup"><span data-stu-id="f5401-104">This resource represents data content of a raw or visual user notification that will be delivered to and consumed by the app client receiving this notification.</span></span>

## <a name="properties"></a><span data-ttu-id="f5401-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f5401-105">Properties</span></span>

| <span data-ttu-id="f5401-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5401-106">Property</span></span>     | <span data-ttu-id="f5401-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5401-107">Type</span></span>        | <span data-ttu-id="f5401-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5401-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f5401-109">rawContent</span><span class="sxs-lookup"><span data-stu-id="f5401-109">rawContent</span></span>|<span data-ttu-id="f5401-110">String</span><span class="sxs-lookup"><span data-stu-id="f5401-110">String</span></span>|<span data-ttu-id="f5401-111">O conteúdo de notificação de uma notificação de usuário bruto que será entregue e consumido pelo cliente de aplicativo em todas as plataformas suportadas (Windows, iOS, Android ou webpush) recebendo esta notificação.</span><span class="sxs-lookup"><span data-stu-id="f5401-111">The notification content of a raw user notification that will be delivered to and consumed by the app client on all supported platforms (Windows, iOS, Android or WebPush) receiving this notification.</span></span> <span data-ttu-id="f5401-112">Pelo menos um dos payloads. RawContent ou Payload. VisualContent precisa ser válido para uma solicitação de notificação POST.</span><span class="sxs-lookup"><span data-stu-id="f5401-112">At least one of Payload.RawContent or Payload.VisualContent needs to be valid for a POST Notification request.</span></span>|
|<span data-ttu-id="f5401-113">visualContent</span><span class="sxs-lookup"><span data-stu-id="f5401-113">visualContent</span></span>|[<span data-ttu-id="f5401-114">visualproperties</span><span class="sxs-lookup"><span data-stu-id="f5401-114">visualProperties</span></span>](visualproperties.md)|<span data-ttu-id="f5401-115">O conteúdo visual de uma notificação de usuário visual, que será consumida pela plataforma de notificação em cada plataforma suportada (Windows, iOS e Android somente) e renderizada para o usuário.</span><span class="sxs-lookup"><span data-stu-id="f5401-115">The visual content of a visual user notification, which will be consumed by the notification platform on each supported platform (Windows, iOS and Android only) and rendered for the user.</span></span> <span data-ttu-id="f5401-116">Pelo menos um dos payloads. RawContent ou Payload. VisualContent precisa ser válido para uma solicitação de notificação POST.</span><span class="sxs-lookup"><span data-stu-id="f5401-116">At least one of Payload.RawContent or Payload.VisualContent needs to be valid for a POST Notification request.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f5401-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f5401-117">JSON representation</span></span>

<span data-ttu-id="f5401-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f5401-118">The following is a JSON representation of the resource.</span></span>

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