---
title: Tipo de recurso de aplicativo
description: Representa o aplicativo Excel que gerencia a pasta de trabalho.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 48ee13a67d97f9c5c1a96a6ef6e104c5629f4108
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517614"
---
# <a name="application-resource-type"></a><span data-ttu-id="2b208-103">Tipo de recurso de aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b208-103">Application resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b208-104">Representa o aplicativo Excel que gerencia a pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2b208-104">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="2b208-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="2b208-105">Methods</span></span>

| <span data-ttu-id="2b208-106">Método</span><span class="sxs-lookup"><span data-stu-id="2b208-106">Method</span></span>           | <span data-ttu-id="2b208-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2b208-107">Return Type</span></span>    |<span data-ttu-id="2b208-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b208-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2b208-109">Obtenha o aplicativo</span><span class="sxs-lookup"><span data-stu-id="2b208-109">Get Application</span></span>](../api/excelapplication-get.md) | [<span data-ttu-id="2b208-110">Application</span><span class="sxs-lookup"><span data-stu-id="2b208-110">Application</span></span>](application.md) |<span data-ttu-id="2b208-111">Leia as propriedades e os relacionamentos do objeto application.</span><span class="sxs-lookup"><span data-stu-id="2b208-111">Read properties and relationships of application object.</span></span>|
|[<span data-ttu-id="2b208-112">Calculate</span><span class="sxs-lookup"><span data-stu-id="2b208-112">Calculate</span></span>](../api/excelapplication-calculate.md)|<span data-ttu-id="2b208-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2b208-113">None</span></span>|<span data-ttu-id="2b208-114">Recalcula todas as pastas de trabalho abertas no Excel no momento.</span><span class="sxs-lookup"><span data-stu-id="2b208-114">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="2b208-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2b208-115">Properties</span></span>
| <span data-ttu-id="2b208-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b208-116">Property</span></span>     | <span data-ttu-id="2b208-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b208-117">Type</span></span>   |<span data-ttu-id="2b208-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b208-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b208-119">calculationMode</span><span class="sxs-lookup"><span data-stu-id="2b208-119">calculationMode</span></span>|<span data-ttu-id="2b208-120">string</span><span class="sxs-lookup"><span data-stu-id="2b208-120">string</span></span>|<span data-ttu-id="2b208-121">Retorna o modo de cálculo usado na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2b208-121">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="2b208-122">Os valores possíveis são: `Automatic`, `AutomaticExceptTables`, `Manual`.</span><span class="sxs-lookup"><span data-stu-id="2b208-122">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span> <span data-ttu-id="2b208-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2b208-123">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b208-124">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="2b208-124">Relationships</span></span>
<span data-ttu-id="2b208-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2b208-125">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2b208-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2b208-126">JSON representation</span></span>

<span data-ttu-id="2b208-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2b208-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.application"
}-->

```json
{
  "calculationMode": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/excelapplication.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
