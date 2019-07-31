---
title: tipo de recurso synchronizationJobRestartCriteria
description: 'Define o escopo da ação [synchronizationJob: reiniciar](../api/synchronization_synchronizationjob_restart.md) .'
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8fb363b74f1daff678d0751aca4a9033b01d9832
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964652"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="0368b-103">tipo de recurso synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="0368b-103">synchronizationJobRestartCriteria resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0368b-104">Define o escopo da ação [synchronizationJob: reiniciar](../api/synchronization-synchronizationjob-restart.md) .</span><span class="sxs-lookup"><span data-stu-id="0368b-104">Defines the scope of the [synchronizationJob: restart](../api/synchronization-synchronizationjob-restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="0368b-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0368b-105">Properties</span></span>
| <span data-ttu-id="0368b-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0368b-106">Property</span></span>     | <span data-ttu-id="0368b-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="0368b-107">Type</span></span>   |<span data-ttu-id="0368b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0368b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0368b-109">resetScope</span><span class="sxs-lookup"><span data-stu-id="0368b-109">resetScope</span></span>|<span data-ttu-id="0368b-110">String</span><span class="sxs-lookup"><span data-stu-id="0368b-110">String</span></span>| <span data-ttu-id="0368b-111">Combinação separada por vírgula dos seguintes `Full`valores:, `QuarantineState`, `Watermark`, `Escrows`,. `ConnectorDataStore`</span><span class="sxs-lookup"><span data-stu-id="0368b-111">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="0368b-112">Use `Full` se você quiser todas as opções.</span><span class="sxs-lookup"><span data-stu-id="0368b-112">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0368b-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0368b-113">JSON representation</span></span>

<span data-ttu-id="0368b-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0368b-114">The following is a JSON representation of the resource.</span></span>

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
