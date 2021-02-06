---
title: Tipo de recurso synchronizationJobRestartCriteria
description: 'Define o escopo da ação synchronizationJob: restart.'
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: ef15c9322c553d0eedb977c3f01ed5de2823e844
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136497"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="ea113-103">Tipo de recurso synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="ea113-103">synchronizationJobRestartCriteria resource type</span></span>

<span data-ttu-id="ea113-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea113-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea113-105">Define o escopo da ação [synchronizationJob: restart.](../api/synchronization-synchronizationjob-restart.md)</span><span class="sxs-lookup"><span data-stu-id="ea113-105">Defines the scope of the [synchronizationJob: restart](../api/synchronization-synchronizationjob-restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="ea113-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea113-106">Properties</span></span>
| <span data-ttu-id="ea113-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea113-107">Property</span></span>     | <span data-ttu-id="ea113-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea113-108">Type</span></span>   |<span data-ttu-id="ea113-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea113-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea113-110">resetScope</span><span class="sxs-lookup"><span data-stu-id="ea113-110">resetScope</span></span>|<span data-ttu-id="ea113-111">String</span><span class="sxs-lookup"><span data-stu-id="ea113-111">String</span></span>| <span data-ttu-id="ea113-112">Combinação separada por vírgulas dos seguintes valores: `Full` , `QuarantineState` , , `Watermark` `Escrows` `ConnectorDataStore` .</span><span class="sxs-lookup"><span data-stu-id="ea113-112">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="ea113-113">Use `Full` se quiser todas as opções.</span><span class="sxs-lookup"><span data-stu-id="ea113-113">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ea113-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea113-114">JSON representation</span></span>

<span data-ttu-id="ea113-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea113-115">The following is a JSON representation of the resource.</span></span>

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


