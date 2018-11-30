---
title: tipo de recurso de notificação
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: c09927cbe133c945b83a3bfc1b0eb74ef00bce2b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039595"
---
# <a name="notification-resource-type"></a><span data-ttu-id="91baf-103">tipo de recurso de notificação</span><span class="sxs-lookup"><span data-stu-id="91baf-103">notification resource type</span></span>

> <span data-ttu-id="91baf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="91baf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91baf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="91baf-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="91baf-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="91baf-106">Properties</span></span>
| <span data-ttu-id="91baf-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91baf-107">Property</span></span>       | <span data-ttu-id="91baf-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="91baf-108">Type</span></span>    | <span data-ttu-id="91baf-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="91baf-109">Description</span></span>                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| <span data-ttu-id="91baf-110">changeType</span><span class="sxs-lookup"><span data-stu-id="91baf-110">changeType</span></span>     | <span data-ttu-id="91baf-111">String</span><span class="sxs-lookup"><span data-stu-id="91baf-111">String</span></span>  | <span data-ttu-id="91baf-112">Os valores possíveis são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="91baf-112">Possible values are: `created`, `updated`, `deleted`.</span></span>      |
| <span data-ttu-id="91baf-113">recurso</span><span class="sxs-lookup"><span data-stu-id="91baf-113">resource</span></span>       | <span data-ttu-id="91baf-114">String</span><span class="sxs-lookup"><span data-stu-id="91baf-114">String</span></span>  | <span data-ttu-id="91baf-115">URI do recurso que foi alterado.</span><span class="sxs-lookup"><span data-stu-id="91baf-115">URI of the resource that was changed.</span></span>                      |

> <span data-ttu-id="91baf-116">**Observação:** `resourceData` está disponível como dados adicionais.</span><span class="sxs-lookup"><span data-stu-id="91baf-116">**Note:** `resourceData` is available as additional data.</span></span> <span data-ttu-id="91baf-117">É uma entidade ou Collection(entity) dependendo do número de pacotes de notificação de alterações.</span><span class="sxs-lookup"><span data-stu-id="91baf-117">It is an entity or Collection(entity) depending on the number of changes packaged in the notification.</span></span>

## <a name="json-representation"></a><span data-ttu-id="91baf-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="91baf-118">JSON representation</span></span>

<span data-ttu-id="91baf-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="91baf-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "resourceData"
  ],
  "@odata.type": "microsoft.graph.commsNotification",
  "openType": true
}-->
```json
{
  "changeType": "created | updated | deleted",
  "resource": "String"
}
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications",
  "truncated": true
}-->
```json
{
  "value": [
    {
      "changeType": "created",
      "resource": "/app/calls/1D6DE2D4-CD51-4309-8DAA-70768651088E",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "id": "1D6DE2D4-CD51-4309-8DAA-70768651088E",
        "state": "incoming"
      }
    }
  ]
}
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications",
  "truncated": true
}-->
```json
{
  "value": [
    {
      "changeType": "created",
      "resource": "/app/calls/1D6DE2D4-CD51-4309-8DAA-70768651088E/participants",
      "resourceData": [
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
        },
        {
          "@odata.type": "#microsoft.graph.participant",
          "id": "8fcb5dbc-d5aa-4681-8e31-b001d5168d79"
        }
      ]
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->