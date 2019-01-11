---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: DefaultColumnValue
localization_priority: Normal
ms.openlocfilehash: 400fc25bf38f12db2be8cef21ddc351316d1265b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810588"
---
# <a name="defaultcolumnvalue-resource-type"></a><span data-ttu-id="f773f-102">Tipo de recurso DefaultColumnValue</span><span class="sxs-lookup"><span data-stu-id="f773f-102">DefaultColumnValue resource type</span></span>

<span data-ttu-id="f773f-103">**defaultColumnValue** em um recurso [columnDefinition](columndefinition.md) especifica o valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="f773f-103">The **defaultColumnValue** on a [columnDefinition](columndefinition.md) resource specifies the default value for this column.</span></span>
<span data-ttu-id="f773f-104">O valor padrão pode ser especificado tanto diretamente ou como uma fórmula.</span><span class="sxs-lookup"><span data-stu-id="f773f-104">The default value can either be specified directly or as a formula.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f773f-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f773f-105">JSON representation</span></span>

<span data-ttu-id="f773f-106">Aqui está uma representação JSON de um recurso **defaultColumnValue**.</span><span class="sxs-lookup"><span data-stu-id="f773f-106">Here is a JSON representation of a **defaultColumnValue** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a><span data-ttu-id="f773f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f773f-107">Properties</span></span>

| <span data-ttu-id="f773f-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="f773f-108">Property name</span></span> | <span data-ttu-id="f773f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f773f-109">Type</span></span>   | <span data-ttu-id="f773f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f773f-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="f773f-111">**formula**</span><span class="sxs-lookup"><span data-stu-id="f773f-111">**formula**</span></span>   | <span data-ttu-id="f773f-112">string</span><span class="sxs-lookup"><span data-stu-id="f773f-112">string</span></span> | <span data-ttu-id="f773f-113">A fórmula usada para calcular o valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="f773f-113">The formula used to compute the default value for this column.</span></span>
| <span data-ttu-id="f773f-114">**value**</span><span class="sxs-lookup"><span data-stu-id="f773f-114">**value**</span></span>     | <span data-ttu-id="f773f-115">string</span><span class="sxs-lookup"><span data-stu-id="f773f-115">string</span></span> | <span data-ttu-id="f773f-116">O valor direto para usar como o valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="f773f-116">The direct value to use as the default value for this column.</span></span>

<span data-ttu-id="f773f-117">Somente uma **fórmula** ou um **valor** pode ser especificado por vez.</span><span class="sxs-lookup"><span data-stu-id="f773f-117">Only one of **formula** or **value** may be specified at a time.</span></span>

<span data-ttu-id="f773f-118">As fórmulas do SharePoint usam uma sintaxe semelhante a fórmulas do Excel.</span><span class="sxs-lookup"><span data-stu-id="f773f-118">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="f773f-119">Consulte [Exemplos de fórmulas comuns em listas do SharePoint][SPFormulas] para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="f773f-119">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue"
} -->
