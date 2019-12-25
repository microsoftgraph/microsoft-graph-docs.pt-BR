---
title: tipo de recurso commsNotification
description: Tipo de base de notificação de comunicação publicado por servidores de comunicação para notificar as alterações.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1752bbe46ee7795bd71df2089dadf6a975ccae26
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870922"
---
# <a name="commsnotification-resource-type"></a><span data-ttu-id="321fa-103">tipo de recurso commsNotification</span><span class="sxs-lookup"><span data-stu-id="321fa-103">commsNotification resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="321fa-104">Tipo de base de notificação de comunicação publicado por servidores de comunicação para notificar as alterações.</span><span class="sxs-lookup"><span data-stu-id="321fa-104">Communications notification base type that is published by Communications servers to notify changes.</span></span>

## <a name="properties"></a><span data-ttu-id="321fa-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="321fa-105">Properties</span></span>
| <span data-ttu-id="321fa-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="321fa-106">Property</span></span>       | <span data-ttu-id="321fa-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="321fa-107">Type</span></span>    | <span data-ttu-id="321fa-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="321fa-108">Description</span></span>                                                |
|:---------------|:--------|:-----------------------------------------------------------|
| <span data-ttu-id="321fa-109">changeType</span><span class="sxs-lookup"><span data-stu-id="321fa-109">changeType</span></span>     | <span data-ttu-id="321fa-110">String</span><span class="sxs-lookup"><span data-stu-id="321fa-110">String</span></span>  | <span data-ttu-id="321fa-111">Os valores possíveis são: `created`, `updated`, `deleted`.</span><span class="sxs-lookup"><span data-stu-id="321fa-111">Possible values are: `created`, `updated`, `deleted`.</span></span>      |
| <span data-ttu-id="321fa-112">Resourceurl pela</span><span class="sxs-lookup"><span data-stu-id="321fa-112">resourceUrl</span></span>       | <span data-ttu-id="321fa-113">String</span><span class="sxs-lookup"><span data-stu-id="321fa-113">String</span></span>  | <span data-ttu-id="321fa-114">URI do recurso que foi alterado.</span><span class="sxs-lookup"><span data-stu-id="321fa-114">URI of the resource that was changed.</span></span>                      |

> <span data-ttu-id="321fa-115">**Observação:** `resourceData` está disponível como dados adicionais.</span><span class="sxs-lookup"><span data-stu-id="321fa-115">**Note:** `resourceData` is available as additional data.</span></span> <span data-ttu-id="321fa-116">É uma entidade ou uma coleção de entidades, dependendo do número de alterações empacotadas na notificação.</span><span class="sxs-lookup"><span data-stu-id="321fa-116">It is either an entity or a collection of entities depending on the number of changes packaged in the notification.</span></span>

## <a name="json-representation"></a><span data-ttu-id="321fa-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="321fa-117">JSON representation</span></span>

<span data-ttu-id="321fa-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="321fa-118">The following is a JSON representation of the resource.</span></span>

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
