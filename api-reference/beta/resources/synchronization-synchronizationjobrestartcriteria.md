---
title: tipo de recurso de synchronizationJobRestartCriteria
description: 'Define o escopo do [synchronizationJob: reiniciar](../api/synchronization_synchronizationjob_restart.md) ação.'
localization_priority: Normal
ms.openlocfilehash: 960bfa56d0bb6921ca971722d894d1b837bfab49
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572301"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="f0824-103">tipo de recurso de synchronizationJobRestartCriteria</span><span class="sxs-lookup"><span data-stu-id="f0824-103">synchronizationJobRestartCriteria resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0824-104">Define o escopo do [synchronizationJob: reiniciar](../api/synchronization-synchronizationjob-restart.md) ação.</span><span class="sxs-lookup"><span data-stu-id="f0824-104">Defines the scope of the [synchronizationJob: restart](../api/synchronization-synchronizationjob-restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="f0824-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0824-105">Properties</span></span>
| <span data-ttu-id="f0824-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0824-106">Property</span></span>     | <span data-ttu-id="f0824-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0824-107">Type</span></span>   |<span data-ttu-id="f0824-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0824-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0824-109">resetScope</span><span class="sxs-lookup"><span data-stu-id="f0824-109">resetScope</span></span>|<span data-ttu-id="f0824-110">String</span><span class="sxs-lookup"><span data-stu-id="f0824-110">String</span></span>| <span data-ttu-id="f0824-111">Combinação de separada por vírgulas dos seguintes valores: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span><span class="sxs-lookup"><span data-stu-id="f0824-111">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="f0824-112">Uso `Full` se desejar que todas as opções.</span><span class="sxs-lookup"><span data-stu-id="f0824-112">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0824-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0824-113">JSON representation</span></span>

<span data-ttu-id="f0824-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f0824-114">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationjobrestartcriteria.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
