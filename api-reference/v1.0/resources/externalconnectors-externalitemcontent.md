---
title: Tipo de recurso externalItemContent
description: O conteúdo de um item indexado por meio de Pesquisa da Microsoft conexão.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 4dd853ca32c918988f2f99e1f1238d9ac937da02
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467190"
---
# <a name="externalitemcontent-resource-type"></a><span data-ttu-id="79256-103">Tipo de recurso externalItemContent</span><span class="sxs-lookup"><span data-stu-id="79256-103">externalItemContent resource type</span></span>

<span data-ttu-id="79256-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="79256-104">Namespace: microsoft.graph.externalConnectors</span></span>

<span data-ttu-id="79256-105">O conteúdo de [um externalItem](externalconnectors-externalitem.md) indexado por meio de uma conexão Pesquisa da Microsoft [.](externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="79256-105">The content of an [externalItem](externalconnectors-externalitem.md) indexed via a Microsoft Search [connection](externalconnectors-externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="79256-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79256-106">Properties</span></span>
|<span data-ttu-id="79256-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79256-107">Property</span></span>|<span data-ttu-id="79256-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="79256-108">Type</span></span>|<span data-ttu-id="79256-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="79256-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79256-110">type</span><span class="sxs-lookup"><span data-stu-id="79256-110">type</span></span>|<span data-ttu-id="79256-111">microsoft.graph.externalConnectors.externalItemContentType</span><span class="sxs-lookup"><span data-stu-id="79256-111">microsoft.graph.externalConnectors.externalItemContentType</span></span>|<span data-ttu-id="79256-112">O tipo de conteúdo na propriedade value.</span><span class="sxs-lookup"><span data-stu-id="79256-112">The type of content in the value property.</span></span> <span data-ttu-id="79256-113">Os valores possíveis são: `text`, `html`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="79256-113">Possible values are: `text`, `html`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="79256-114">value</span><span class="sxs-lookup"><span data-stu-id="79256-114">value</span></span>|<span data-ttu-id="79256-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79256-115">String</span></span>|<span data-ttu-id="79256-116">O conteúdo do externalItem.</span><span class="sxs-lookup"><span data-stu-id="79256-116">The content for the externalItem.</span></span> <span data-ttu-id="79256-117">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79256-117">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79256-118">Relações</span><span class="sxs-lookup"><span data-stu-id="79256-118">Relationships</span></span>
<span data-ttu-id="79256-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="79256-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="79256-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79256-120">JSON representation</span></span>
<span data-ttu-id="79256-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="79256-121">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.externalItemContent"
}
-->
``` json
{
  "value": "String",
  "type": "String"
}
```

