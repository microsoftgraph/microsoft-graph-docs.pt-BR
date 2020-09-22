---
author: daspek
description: defaultColumnValue em um recurso columnDefinition especifica o valor padrão dessa coluna.
ms.date: 09/12/2017
title: DefaultColumnValue
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: b6e161f6d0e0c38ab6a1aeef7d17894ba11141c3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049951"
---
# <a name="defaultcolumnvalue-resource-type"></a><span data-ttu-id="5177d-103">Tipo de recurso DefaultColumnValue</span><span class="sxs-lookup"><span data-stu-id="5177d-103">DefaultColumnValue resource type</span></span>

<span data-ttu-id="5177d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5177d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5177d-105">**defaultColumnValue** em um recurso [columnDefinition](columndefinition.md) especifica o valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="5177d-105">The **defaultColumnValue** on a [columnDefinition](columndefinition.md) resource specifies the default value for this column.</span></span>
<span data-ttu-id="5177d-106">O valor padrão pode ser especificado tanto diretamente ou como uma fórmula.</span><span class="sxs-lookup"><span data-stu-id="5177d-106">The default value can either be specified directly or as a formula.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5177d-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5177d-107">JSON representation</span></span>

<span data-ttu-id="5177d-108">Aqui está uma representação JSON de um recurso **defaultColumnValue**.</span><span class="sxs-lookup"><span data-stu-id="5177d-108">Here is a JSON representation of a **defaultColumnValue** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a><span data-ttu-id="5177d-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5177d-109">Properties</span></span>

| <span data-ttu-id="5177d-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="5177d-110">Property name</span></span> | <span data-ttu-id="5177d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="5177d-111">Type</span></span>   | <span data-ttu-id="5177d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="5177d-112">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="5177d-113">**formula**</span><span class="sxs-lookup"><span data-stu-id="5177d-113">**formula**</span></span>   | <span data-ttu-id="5177d-114">string</span><span class="sxs-lookup"><span data-stu-id="5177d-114">string</span></span> | <span data-ttu-id="5177d-115">A fórmula usada para calcular o valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="5177d-115">The formula used to compute the default value for this column.</span></span>
| <span data-ttu-id="5177d-116">**value**</span><span class="sxs-lookup"><span data-stu-id="5177d-116">**value**</span></span>     | <span data-ttu-id="5177d-117">string</span><span class="sxs-lookup"><span data-stu-id="5177d-117">string</span></span> | <span data-ttu-id="5177d-118">O valor direto para usar como o valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="5177d-118">The direct value to use as the default value for this column.</span></span>

<span data-ttu-id="5177d-119">Somente uma **fórmula** ou um **valor** pode ser especificado por vez.</span><span class="sxs-lookup"><span data-stu-id="5177d-119">Only one of **formula** or **value** may be specified at a time.</span></span>

<span data-ttu-id="5177d-120">As fórmulas do SharePoint usam uma sintaxe semelhante a fórmulas do Excel.</span><span class="sxs-lookup"><span data-stu-id="5177d-120">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="5177d-121">Consulte [Exemplos de fórmulas comuns em listas do SharePoint][SPFormulas] para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="5177d-121">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue",
  "suppressions": []
}
-->


