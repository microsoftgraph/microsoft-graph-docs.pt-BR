---
title: tipo de recurso commsNotifications
description: Lista de notificações usadas pelos servidores de comunicação para o envio de várias notificações em um único lote.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b5cbd2e2e2875a3e2ab207925a11fa258ad117f2
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913237"
---
# <a name="commsnotifications-resource-type"></a><span data-ttu-id="b9dbb-103">tipo de recurso commsNotifications</span><span class="sxs-lookup"><span data-stu-id="b9dbb-103">commsNotifications resource type</span></span>

<span data-ttu-id="b9dbb-104">Lista de notificações usadas pelos servidores de comunicação para o envio de várias notificações em um único lote.</span><span class="sxs-lookup"><span data-stu-id="b9dbb-104">List of notifications used by the Communications servers for sending multiple notifications in a single batch.</span></span>

## <a name="properties"></a><span data-ttu-id="b9dbb-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b9dbb-105">Properties</span></span>

| <span data-ttu-id="b9dbb-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9dbb-106">Property</span></span>       | <span data-ttu-id="b9dbb-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9dbb-107">Type</span></span>                                                 | <span data-ttu-id="b9dbb-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9dbb-108">Description</span></span>                                   |
|:---------------|:-----------------------------------------------------|:----------------------------------------------|
| <span data-ttu-id="b9dbb-109">valor</span><span class="sxs-lookup"><span data-stu-id="b9dbb-109">value</span></span>          | <span data-ttu-id="b9dbb-110">coleção [commsNotification](commsnotification.md)</span><span class="sxs-lookup"><span data-stu-id="b9dbb-110">[commsNotification](commsnotification.md) collection</span></span> | <span data-ttu-id="b9dbb-111">A notificação de uma alteração no recurso.</span><span class="sxs-lookup"><span data-stu-id="b9dbb-111">The notification of a change in the resource.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b9dbb-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b9dbb-112">JSON representation</span></span>

<span data-ttu-id="b9dbb-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b9dbb-113">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "commsNotifications resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
