---
title: tipo de recurso de commsNotification
description: Comunicações notificação tipo base publicado pelos servidores do Communications Server para notificar mudanças.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e5b929997cf17d13043264d42421418321aae84e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977693"
---
# <a name="commsnotification-resource-type"></a><span data-ttu-id="d5bd4-103">tipo de recurso de commsNotification</span><span class="sxs-lookup"><span data-stu-id="d5bd4-103">commsNotification resource type</span></span>

> <span data-ttu-id="d5bd4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d5bd4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5bd4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d5bd4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d5bd4-106">Comunicações notificação tipo base publicado pelos servidores do Communications Server para notificar mudanças.</span><span class="sxs-lookup"><span data-stu-id="d5bd4-106">Communications notification base type that is published by Communications servers to notify changes.</span></span>

## <a name="properties"></a><span data-ttu-id="d5bd4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5bd4-107">Properties</span></span>
| <span data-ttu-id="d5bd4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5bd4-108">Property</span></span>       | <span data-ttu-id="d5bd4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5bd4-109">Type</span></span>    | <span data-ttu-id="d5bd4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5bd4-110">Description</span></span>                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| <span data-ttu-id="d5bd4-111">changeType</span><span class="sxs-lookup"><span data-stu-id="d5bd4-111">changeType</span></span>     | <span data-ttu-id="d5bd4-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5bd4-112">String</span></span>  | <span data-ttu-id="d5bd4-113">Os valores possíveis são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="d5bd4-113">Possible values are: `created`, `updated`, `deleted`.</span></span>      |
| <span data-ttu-id="d5bd4-114">recurso</span><span class="sxs-lookup"><span data-stu-id="d5bd4-114">resource</span></span>       | <span data-ttu-id="d5bd4-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5bd4-115">String</span></span>  | <span data-ttu-id="d5bd4-116">URI do recurso que foi alterado.</span><span class="sxs-lookup"><span data-stu-id="d5bd4-116">URI of the resource that was changed.</span></span>                      |

> <span data-ttu-id="d5bd4-117">**Observação:** `resourceData` está disponível como dados adicionais.</span><span class="sxs-lookup"><span data-stu-id="d5bd4-117">**Note:** `resourceData` is available as additional data.</span></span> <span data-ttu-id="d5bd4-118">É uma entidade ou Collection(entity) dependendo do número de pacotes de notificação de alterações.</span><span class="sxs-lookup"><span data-stu-id="d5bd4-118">It is an entity or Collection(entity) depending on the number of changes packaged in the notification.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5bd4-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5bd4-119">JSON representation</span></span>

<span data-ttu-id="d5bd4-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5bd4-120">The following is a JSON representation of the resource.</span></span>

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
  "description": "commsNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
