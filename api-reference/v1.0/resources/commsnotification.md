---
title: tipo de recurso commsNotification
description: Tipo de base de notificação de comunicação publicado por servidores de comunicação para notificar as alterações.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2276547b99e297f1e015e12f9ed2254d3cb4632d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018974"
---
# <a name="commsnotification-resource-type"></a><span data-ttu-id="9f7e5-103">tipo de recurso commsNotification</span><span class="sxs-lookup"><span data-stu-id="9f7e5-103">commsNotification resource type</span></span>

<span data-ttu-id="9f7e5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f7e5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9f7e5-105">Tipo de base de notificação de comunicação publicado por servidores de comunicação para notificar as alterações.</span><span class="sxs-lookup"><span data-stu-id="9f7e5-105">Communications notification base type that is published by Communications servers to notify changes.</span></span>

## <a name="properties"></a><span data-ttu-id="9f7e5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9f7e5-106">Properties</span></span>
| <span data-ttu-id="9f7e5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f7e5-107">Property</span></span>       | <span data-ttu-id="9f7e5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f7e5-108">Type</span></span>    | <span data-ttu-id="9f7e5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f7e5-109">Description</span></span>                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| <span data-ttu-id="9f7e5-110">changeType</span><span class="sxs-lookup"><span data-stu-id="9f7e5-110">changeType</span></span>     | <span data-ttu-id="9f7e5-111">String</span><span class="sxs-lookup"><span data-stu-id="9f7e5-111">String</span></span>  | <span data-ttu-id="9f7e5-112">Os valores possíveis são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="9f7e5-112">Possible values are: `created`, `updated`, `deleted`.</span></span>      |
| <span data-ttu-id="9f7e5-113">Resourceurl pela</span><span class="sxs-lookup"><span data-stu-id="9f7e5-113">resourceUrl</span></span>       | <span data-ttu-id="9f7e5-114">String</span><span class="sxs-lookup"><span data-stu-id="9f7e5-114">String</span></span>  | <span data-ttu-id="9f7e5-115">URI do recurso que foi alterado.</span><span class="sxs-lookup"><span data-stu-id="9f7e5-115">URI of the resource that was changed.</span></span>                      |

> <span data-ttu-id="9f7e5-116">**Observação:** `resourceData` está disponível como dados adicionais.</span><span class="sxs-lookup"><span data-stu-id="9f7e5-116">**Note:** `resourceData` is available as additional data.</span></span> <span data-ttu-id="9f7e5-117">É uma entidade ou uma coleção de entidades, dependendo do número de alterações empacotadas na notificação.</span><span class="sxs-lookup"><span data-stu-id="9f7e5-117">It is either an entity or a collection of entities depending on the number of changes packaged in the notification.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f7e5-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9f7e5-118">JSON representation</span></span>

<span data-ttu-id="9f7e5-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9f7e5-119">The following is a JSON representation of the resource.</span></span>

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
  "@odata.type": "#microsoft.graph.commsNotification",
  "changeType": "created | updated | deleted",
  "resourceUrl": "String"
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
  "suppressions": []
}
-->

