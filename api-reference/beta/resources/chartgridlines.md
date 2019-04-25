---
title: Tipo de recurso ChartGridlines
description: Representa linhas de grade principais ou secundárias em um eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 852b52fd70e619b8720ef56fb0e857fb499f0abf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543690"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="f2769-103">Tipo de recurso ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="f2769-103">ChartGridlines resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2769-104">Representa linhas de grade principais ou secundárias em um eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="f2769-104">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="f2769-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="f2769-105">Methods</span></span>

| <span data-ttu-id="f2769-106">Método</span><span class="sxs-lookup"><span data-stu-id="f2769-106">Method</span></span>           | <span data-ttu-id="f2769-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f2769-107">Return Type</span></span>    |<span data-ttu-id="f2769-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2769-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f2769-109">Get ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="f2769-109">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="f2769-110">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="f2769-110">ChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="f2769-111">Leia as propriedades e os relacionamentos do objeto chartGridlines.</span><span class="sxs-lookup"><span data-stu-id="f2769-111">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="f2769-112">Update</span><span class="sxs-lookup"><span data-stu-id="f2769-112">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="f2769-113">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="f2769-113">ChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="f2769-114">Atualize o objeto ChartGridlines.</span><span class="sxs-lookup"><span data-stu-id="f2769-114">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f2769-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f2769-115">Properties</span></span>
| <span data-ttu-id="f2769-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2769-116">Property</span></span>     | <span data-ttu-id="f2769-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2769-117">Type</span></span>   |<span data-ttu-id="f2769-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2769-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2769-119">visible</span><span class="sxs-lookup"><span data-stu-id="f2769-119">visible</span></span>|<span data-ttu-id="f2769-120">booliano</span><span class="sxs-lookup"><span data-stu-id="f2769-120">boolean</span></span>|<span data-ttu-id="f2769-121">Valor booliano que determina se as linhas de grade do eixo ficam visíveis ou não.</span><span class="sxs-lookup"><span data-stu-id="f2769-121">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2769-122">Relações</span><span class="sxs-lookup"><span data-stu-id="f2769-122">Relationships</span></span>
| <span data-ttu-id="f2769-123">Relação</span><span class="sxs-lookup"><span data-stu-id="f2769-123">Relationship</span></span> | <span data-ttu-id="f2769-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2769-124">Type</span></span>   |<span data-ttu-id="f2769-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2769-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2769-126">format</span><span class="sxs-lookup"><span data-stu-id="f2769-126">format</span></span>|[<span data-ttu-id="f2769-127">ChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="f2769-127">ChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="f2769-p101">Representa a formatação de linhas de grade do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f2769-p101">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f2769-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f2769-130">JSON representation</span></span>

<span data-ttu-id="f2769-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f2769-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartGridLines"
}-->

```json
{
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartgridlines.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
