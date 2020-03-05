---
title: tipo de recurso synchronizationJobRestartCriteria
description: 'Define o escopo da ação [synchronizationJob: reiniciar](../api/synchronization_synchronizationjob_restart.md) .'
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8c8992104493e7f59b1ddc74c7128dda50b2bfd9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520062"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="b469d-103">tipo de recurso synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="b469d-103">synchronizationJobRestartCriteria resource type</span></span>

<span data-ttu-id="b469d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b469d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b469d-105">Define o escopo da ação [synchronizationJob: reiniciar](../api/synchronization-synchronizationjob-restart.md) .</span><span class="sxs-lookup"><span data-stu-id="b469d-105">Defines the scope of the [synchronizationJob: restart](../api/synchronization-synchronizationjob-restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="b469d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b469d-106">Properties</span></span>
| <span data-ttu-id="b469d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b469d-107">Property</span></span>     | <span data-ttu-id="b469d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b469d-108">Type</span></span>   |<span data-ttu-id="b469d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b469d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b469d-110">resetScope</span><span class="sxs-lookup"><span data-stu-id="b469d-110">resetScope</span></span>|<span data-ttu-id="b469d-111">String</span><span class="sxs-lookup"><span data-stu-id="b469d-111">String</span></span>| <span data-ttu-id="b469d-112">Combinação separada por vírgula dos seguintes `Full`valores:, `QuarantineState`, `Watermark`, `Escrows`,. `ConnectorDataStore`</span><span class="sxs-lookup"><span data-stu-id="b469d-112">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="b469d-113">Use `Full` se você quiser todas as opções.</span><span class="sxs-lookup"><span data-stu-id="b469d-113">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b469d-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b469d-114">JSON representation</span></span>

<span data-ttu-id="b469d-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b469d-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJobRestartCriteria"
}-->

```json
{
  "resetScope": "String"
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
