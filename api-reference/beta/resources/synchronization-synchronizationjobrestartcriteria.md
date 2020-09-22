---
title: tipo de recurso synchronizationJobRestartCriteria
description: 'Define o escopo da ação synchronizationJob: reiniciar.'
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 82d671f411725a1e6537580205c7298cf887e3a1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023839"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="48b2d-103">tipo de recurso synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="48b2d-103">synchronizationJobRestartCriteria resource type</span></span>

<span data-ttu-id="48b2d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48b2d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48b2d-105">Define o escopo da ação [synchronizationJob: reiniciar](../api/synchronization-synchronizationjob-restart.md) .</span><span class="sxs-lookup"><span data-stu-id="48b2d-105">Defines the scope of the [synchronizationJob: restart](../api/synchronization-synchronizationjob-restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="48b2d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48b2d-106">Properties</span></span>
| <span data-ttu-id="48b2d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48b2d-107">Property</span></span>     | <span data-ttu-id="48b2d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="48b2d-108">Type</span></span>   |<span data-ttu-id="48b2d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="48b2d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="48b2d-110">resetScope</span><span class="sxs-lookup"><span data-stu-id="48b2d-110">resetScope</span></span>|<span data-ttu-id="48b2d-111">String</span><span class="sxs-lookup"><span data-stu-id="48b2d-111">String</span></span>| <span data-ttu-id="48b2d-112">Combinação separada por vírgula dos seguintes valores: `Full` ,, `QuarantineState` , `Watermark` , `Escrows` `ConnectorDataStore` .</span><span class="sxs-lookup"><span data-stu-id="48b2d-112">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="48b2d-113">Use `Full` se você quiser todas as opções.</span><span class="sxs-lookup"><span data-stu-id="48b2d-113">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="48b2d-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48b2d-114">JSON representation</span></span>

<span data-ttu-id="48b2d-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="48b2d-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJobRestartCriteria"
}-->

```json
{
    "criteria": {
        "resetScope": "String"
    }
}


```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJobRestartCriteria resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


