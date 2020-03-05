---
title: tipo de recurso commsNotification
description: Tipo de base de notificação de comunicação publicado por servidores de comunicação para notificar as alterações.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4ec3df8bc56e6164af3b7752333d28bd10665d67
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507601"
---
# <a name="commsnotification-resource-type"></a><span data-ttu-id="3f8f7-103">tipo de recurso commsNotification</span><span class="sxs-lookup"><span data-stu-id="3f8f7-103">commsNotification resource type</span></span>

<span data-ttu-id="3f8f7-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3f8f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f8f7-105">Tipo de base de notificação de comunicação publicado por servidores de comunicação para notificar as alterações.</span><span class="sxs-lookup"><span data-stu-id="3f8f7-105">Communications notification base type that is published by Communications servers to notify changes.</span></span>

## <a name="properties"></a><span data-ttu-id="3f8f7-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3f8f7-106">Properties</span></span>
| <span data-ttu-id="3f8f7-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f8f7-107">Property</span></span>       | <span data-ttu-id="3f8f7-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f8f7-108">Type</span></span>    | <span data-ttu-id="3f8f7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f8f7-109">Description</span></span>                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| <span data-ttu-id="3f8f7-110">changeType</span><span class="sxs-lookup"><span data-stu-id="3f8f7-110">changeType</span></span>     | <span data-ttu-id="3f8f7-111">String</span><span class="sxs-lookup"><span data-stu-id="3f8f7-111">String</span></span>  | <span data-ttu-id="3f8f7-112">Os valores possíveis são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="3f8f7-112">Possible values are: `created`, `updated`, `deleted`.</span></span>      |
| <span data-ttu-id="3f8f7-113">Resourceurl pela</span><span class="sxs-lookup"><span data-stu-id="3f8f7-113">resourceUrl</span></span>       | <span data-ttu-id="3f8f7-114">String</span><span class="sxs-lookup"><span data-stu-id="3f8f7-114">String</span></span>  | <span data-ttu-id="3f8f7-115">URI do recurso que foi alterado.</span><span class="sxs-lookup"><span data-stu-id="3f8f7-115">URI of the resource that was changed.</span></span>                      |

> <span data-ttu-id="3f8f7-116">**Observação:** `resourceData` está disponível como dados adicionais.</span><span class="sxs-lookup"><span data-stu-id="3f8f7-116">**Note:** `resourceData` is available as additional data.</span></span> <span data-ttu-id="3f8f7-117">É uma entidade ou uma coleção de entidades, dependendo do número de alterações empacotadas na notificação.</span><span class="sxs-lookup"><span data-stu-id="3f8f7-117">It is either an entity or a collection of entities depending on the number of changes packaged in the notification.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f8f7-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3f8f7-118">JSON representation</span></span>

<span data-ttu-id="3f8f7-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3f8f7-119">The following is a JSON representation of the resource.</span></span>

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
