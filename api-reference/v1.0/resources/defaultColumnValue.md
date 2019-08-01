---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: DefaultColumnValue
localization_priority: Normal
description: defaultColumnValue em um recurso columnDefinition especifica o valor padrão dessa coluna.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 4a2ddff8de7efb2bb697ffae63d69376588e6ac9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029509"
---
# <a name="defaultcolumnvalue-resource-type"></a><span data-ttu-id="e920a-103">Tipo de recurso DefaultColumnValue</span><span class="sxs-lookup"><span data-stu-id="e920a-103">DefaultColumnValue resource type</span></span>

<span data-ttu-id="e920a-104">**defaultColumnValue** em um recurso [columnDefinition](columndefinition.md) especifica o valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="e920a-104">The **defaultColumnValue** on a [columnDefinition](columndefinition.md) resource specifies the default value for this column.</span></span>
<span data-ttu-id="e920a-105">O valor padrão pode ser especificado tanto diretamente ou como uma fórmula.</span><span class="sxs-lookup"><span data-stu-id="e920a-105">The default value can either be specified directly or as a formula.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e920a-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e920a-106">JSON representation</span></span>

<span data-ttu-id="e920a-107">Aqui está uma representação JSON de um recurso **defaultColumnValue**.</span><span class="sxs-lookup"><span data-stu-id="e920a-107">Here is a JSON representation of a **defaultColumnValue** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a><span data-ttu-id="e920a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e920a-108">Properties</span></span>

| <span data-ttu-id="e920a-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="e920a-109">Property name</span></span> | <span data-ttu-id="e920a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e920a-110">Type</span></span>   | <span data-ttu-id="e920a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e920a-111">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="e920a-112">**formula**</span><span class="sxs-lookup"><span data-stu-id="e920a-112">**formula**</span></span>   | <span data-ttu-id="e920a-113">string</span><span class="sxs-lookup"><span data-stu-id="e920a-113">string</span></span> | <span data-ttu-id="e920a-114">A fórmula usada para calcular o valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="e920a-114">The formula used to compute the default value for this column.</span></span>
| <span data-ttu-id="e920a-115">**value**</span><span class="sxs-lookup"><span data-stu-id="e920a-115">**value**</span></span>     | <span data-ttu-id="e920a-116">string</span><span class="sxs-lookup"><span data-stu-id="e920a-116">string</span></span> | <span data-ttu-id="e920a-117">O valor direto para usar como o valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="e920a-117">The direct value to use as the default value for this column.</span></span>

<span data-ttu-id="e920a-118">Somente uma **fórmula** ou um **valor** pode ser especificado por vez.</span><span class="sxs-lookup"><span data-stu-id="e920a-118">Only one of **formula** or **value** may be specified at a time.</span></span>

<span data-ttu-id="e920a-119">As fórmulas do SharePoint usam uma sintaxe semelhante a fórmulas do Excel.</span><span class="sxs-lookup"><span data-stu-id="e920a-119">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="e920a-120">Consulte [Exemplos de fórmulas comuns em listas do SharePoint][SPFormulas] para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="e920a-120">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue"
} -->
