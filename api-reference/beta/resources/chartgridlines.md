---
title: Tipo de recurso ChartGridlines
description: Representa as linhas de grade principais ou secundárias em um eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 044af64a6b6d41d9d5407678d1bd1e49cbdffe8a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928147"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="3b302-103">Tipo de recurso ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="3b302-103">ChartGridlines resource type</span></span>

> <span data-ttu-id="3b302-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3b302-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b302-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3b302-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3b302-106">Representa linhas de grade principais ou secundárias em um eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="3b302-106">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="3b302-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="3b302-107">Methods</span></span>

| <span data-ttu-id="3b302-108">Método</span><span class="sxs-lookup"><span data-stu-id="3b302-108">Method</span></span>           | <span data-ttu-id="3b302-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3b302-109">Return Type</span></span>    |<span data-ttu-id="3b302-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b302-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3b302-111">Get ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="3b302-111">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="3b302-112">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="3b302-112">ChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="3b302-113">Leia as propriedades e os relacionamentos do objeto chartGridlines.</span><span class="sxs-lookup"><span data-stu-id="3b302-113">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="3b302-114">Update</span><span class="sxs-lookup"><span data-stu-id="3b302-114">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="3b302-115">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="3b302-115">ChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="3b302-116">Atualize o objeto ChartGridlines.</span><span class="sxs-lookup"><span data-stu-id="3b302-116">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3b302-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3b302-117">Properties</span></span>
| <span data-ttu-id="3b302-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b302-118">Property</span></span>     | <span data-ttu-id="3b302-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b302-119">Type</span></span>   |<span data-ttu-id="3b302-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b302-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b302-121">visible</span><span class="sxs-lookup"><span data-stu-id="3b302-121">visible</span></span>|<span data-ttu-id="3b302-122">booliano</span><span class="sxs-lookup"><span data-stu-id="3b302-122">boolean</span></span>|<span data-ttu-id="3b302-123">Valor booliano que determina se as linhas de grade do eixo ficam visíveis ou não.</span><span class="sxs-lookup"><span data-stu-id="3b302-123">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b302-124">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="3b302-124">Relationships</span></span>
| <span data-ttu-id="3b302-125">Relação</span><span class="sxs-lookup"><span data-stu-id="3b302-125">Relationship</span></span> | <span data-ttu-id="3b302-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b302-126">Type</span></span>   |<span data-ttu-id="3b302-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b302-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b302-128">formato</span><span class="sxs-lookup"><span data-stu-id="3b302-128">format</span></span>|[<span data-ttu-id="3b302-129">ChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="3b302-129">ChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="3b302-p102">Representa a formatação de linhas de grade do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3b302-p102">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3b302-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3b302-132">JSON representation</span></span>

<span data-ttu-id="3b302-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3b302-133">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartGridlines resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
