---
title: Tipo de recurso ChartGridlines
description: Representa as linhas de grade principais ou secundárias em um eixo do gráfico.
author: lumine2008
ms.openlocfilehash: 263bbefad519fef8b12080cb7b2bfd74ce1a331f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319555"
---
# <a name="chartgridlines-resource-type"></a><span data-ttu-id="1b69e-103">Tipo de recurso ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="1b69e-103">ChartGridlines resource type</span></span>

> <span data-ttu-id="1b69e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1b69e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b69e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1b69e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1b69e-106">Representa linhas de grade principais ou secundárias em um eixo do gráfico.</span><span class="sxs-lookup"><span data-stu-id="1b69e-106">Represents major or minor gridlines on a chart axis.</span></span>


## <a name="methods"></a><span data-ttu-id="1b69e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="1b69e-107">Methods</span></span>

| <span data-ttu-id="1b69e-108">Método</span><span class="sxs-lookup"><span data-stu-id="1b69e-108">Method</span></span>           | <span data-ttu-id="1b69e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1b69e-109">Return Type</span></span>    |<span data-ttu-id="1b69e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b69e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1b69e-111">Get ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="1b69e-111">Get ChartGridlines</span></span>](../api/chartgridlines-get.md) | [<span data-ttu-id="1b69e-112">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="1b69e-112">ChartGridlines</span></span>](chartgridlines.md) |<span data-ttu-id="1b69e-113">Leia as propriedades e os relacionamentos do objeto chartGridlines.</span><span class="sxs-lookup"><span data-stu-id="1b69e-113">Read properties and relationships of chartGridlines object.</span></span>|
|[<span data-ttu-id="1b69e-114">Update</span><span class="sxs-lookup"><span data-stu-id="1b69e-114">Update</span></span>](../api/chartgridlines-update.md) | [<span data-ttu-id="1b69e-115">ChartGridlines</span><span class="sxs-lookup"><span data-stu-id="1b69e-115">ChartGridlines</span></span>](chartgridlines.md)    |<span data-ttu-id="1b69e-116">Atualize o objeto ChartGridlines.</span><span class="sxs-lookup"><span data-stu-id="1b69e-116">Update ChartGridlines object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1b69e-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b69e-117">Properties</span></span>
| <span data-ttu-id="1b69e-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b69e-118">Property</span></span>     | <span data-ttu-id="1b69e-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b69e-119">Type</span></span>   |<span data-ttu-id="1b69e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b69e-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b69e-121">visible</span><span class="sxs-lookup"><span data-stu-id="1b69e-121">visible</span></span>|<span data-ttu-id="1b69e-122">booliano</span><span class="sxs-lookup"><span data-stu-id="1b69e-122">boolean</span></span>|<span data-ttu-id="1b69e-123">Valor booliano que determina se as linhas de grade do eixo ficam visíveis ou não.</span><span class="sxs-lookup"><span data-stu-id="1b69e-123">Boolean value representing if the axis gridlines are visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b69e-124">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="1b69e-124">Relationships</span></span>
| <span data-ttu-id="1b69e-125">Relação</span><span class="sxs-lookup"><span data-stu-id="1b69e-125">Relationship</span></span> | <span data-ttu-id="1b69e-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b69e-126">Type</span></span>   |<span data-ttu-id="1b69e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b69e-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1b69e-128">formato</span><span class="sxs-lookup"><span data-stu-id="1b69e-128">format</span></span>|[<span data-ttu-id="1b69e-129">ChartGridlinesFormat</span><span class="sxs-lookup"><span data-stu-id="1b69e-129">ChartGridlinesFormat</span></span>](chartgridlinesformat.md)|<span data-ttu-id="1b69e-p102">Representa a formatação de linhas de grade do gráfico. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1b69e-p102">Represents the formatting of chart gridlines. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b69e-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b69e-132">JSON representation</span></span>

<span data-ttu-id="1b69e-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1b69e-133">Here is a JSON representation of the resource.</span></span>

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