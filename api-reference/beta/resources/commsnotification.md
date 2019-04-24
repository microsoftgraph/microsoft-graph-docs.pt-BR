---
title: tipo de recurso commsNotification
description: Tipo de base de notificação de comunicação publicado por servidores de comunicação para notificar as alterações.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2372720976b5d06ffe49c00068625bdb92048674
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460671"
---
# <a name="commsnotification-resource-type"></a><span data-ttu-id="a8c56-103">tipo de recurso commsNotification</span><span class="sxs-lookup"><span data-stu-id="a8c56-103">commsNotification resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8c56-104">Tipo de base de notificação de comunicação publicado por servidores de comunicação para notificar as alterações.</span><span class="sxs-lookup"><span data-stu-id="a8c56-104">Communications notification base type that is published by Communications servers to notify changes.</span></span>

## <a name="properties"></a><span data-ttu-id="a8c56-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8c56-105">Properties</span></span>
| <span data-ttu-id="a8c56-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8c56-106">Property</span></span>       | <span data-ttu-id="a8c56-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8c56-107">Type</span></span>    | <span data-ttu-id="a8c56-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8c56-108">Description</span></span>                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| <span data-ttu-id="a8c56-109">changeType</span><span class="sxs-lookup"><span data-stu-id="a8c56-109">changeType</span></span>     | <span data-ttu-id="a8c56-110">String</span><span class="sxs-lookup"><span data-stu-id="a8c56-110">String</span></span>  | <span data-ttu-id="a8c56-111">Os valores possíveis são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="a8c56-111">Possible values are: `created`, `updated`, `deleted`.</span></span>      |
| <span data-ttu-id="a8c56-112">recurso</span><span class="sxs-lookup"><span data-stu-id="a8c56-112">resource</span></span>       | <span data-ttu-id="a8c56-113">String</span><span class="sxs-lookup"><span data-stu-id="a8c56-113">String</span></span>  | <span data-ttu-id="a8c56-114">URI do recurso que foi alterado.</span><span class="sxs-lookup"><span data-stu-id="a8c56-114">URI of the resource that was changed.</span></span>                      |

> <span data-ttu-id="a8c56-115">**Observação:** `resourceData` está disponível como dados adicionais.</span><span class="sxs-lookup"><span data-stu-id="a8c56-115">**Note:** `resourceData` is available as additional data.</span></span> <span data-ttu-id="a8c56-116">É uma entidade ou coleção (entidade), dependendo do número de alterações empacotadas na notificação.</span><span class="sxs-lookup"><span data-stu-id="a8c56-116">It is an entity or Collection(entity) depending on the number of changes packaged in the notification.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8c56-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8c56-117">JSON representation</span></span>

<span data-ttu-id="a8c56-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8c56-118">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "commsNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/commsnotification.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
