---
title: tipo de recurso de notificações
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 96246491c386971fe18184f26269d4abe3af6e6e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040830"
---
# <a name="notifications-resource-type"></a><span data-ttu-id="da10f-103">tipo de recurso de notificações</span><span class="sxs-lookup"><span data-stu-id="da10f-103">notifications resource type</span></span>

> <span data-ttu-id="da10f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="da10f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da10f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="da10f-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="da10f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da10f-106">Properties</span></span>

| <span data-ttu-id="da10f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da10f-107">Property</span></span>       | <span data-ttu-id="da10f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="da10f-108">Type</span></span>                                       | <span data-ttu-id="da10f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="da10f-109">Description</span></span> |
|:---------------|:-------------------------------------------|:------------|
| <span data-ttu-id="da10f-110">valor</span><span class="sxs-lookup"><span data-stu-id="da10f-110">value</span></span>          | <span data-ttu-id="da10f-111">coleção de [notificação](commsnotification.md)</span><span class="sxs-lookup"><span data-stu-id="da10f-111">[notification](commsnotification.md) collection</span></span> | <span data-ttu-id="da10f-112">A notificação de alteração no recurso.</span><span class="sxs-lookup"><span data-stu-id="da10f-112">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="da10f-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da10f-113">JSON representation</span></span>

<span data-ttu-id="da10f-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="da10f-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "value": [ { "@odata.type": "#microsoft.graph.commsNotification" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->