---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: DefaultColumnValue
ms.openlocfilehash: 3a486b6cc90dffb75343390102ecb3b17576e6fb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037457"
---
# <a name="defaultcolumnvalue-resource-type"></a><span data-ttu-id="ee7d5-102">Tipo de recurso DefaultColumnValue</span><span class="sxs-lookup"><span data-stu-id="ee7d5-102">DefaultColumnValue resource type</span></span>

> <span data-ttu-id="ee7d5-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ee7d5-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ee7d5-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ee7d5-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ee7d5-105">**defaultColumnValue** em um recurso [columnDefinition](columndefinition.md) especifica o valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="ee7d5-105">The **defaultColumnValue** on a [columnDefinition](columndefinition.md) resource specifies the default value for this column.</span></span>
<span data-ttu-id="ee7d5-106">O valor padrão pode ser especificado tanto diretamente ou como uma fórmula.</span><span class="sxs-lookup"><span data-stu-id="ee7d5-106">The default value can either be specified directly or as a formula.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee7d5-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee7d5-107">JSON representation</span></span>

<span data-ttu-id="ee7d5-108">Aqui está uma representação JSON de um recurso **defaultColumnValue**.</span><span class="sxs-lookup"><span data-stu-id="ee7d5-108">Here is a JSON representation of a **defaultColumnValue** resource.</span></span>
<!-- { "blockType": "resource", "@type": "microsoft.graph.defaultColumnValue" } -->

```json
{
  "formula": "=[Column1]+[Column2]+[Column3]",
  "value": "defaultValueString"
}
```

## <a name="properties"></a><span data-ttu-id="ee7d5-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee7d5-109">Properties</span></span>

| <span data-ttu-id="ee7d5-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ee7d5-110">Property name</span></span> | <span data-ttu-id="ee7d5-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee7d5-111">Type</span></span>   | <span data-ttu-id="ee7d5-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee7d5-112">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="ee7d5-113">**formula**</span><span class="sxs-lookup"><span data-stu-id="ee7d5-113">**formula**</span></span>   | <span data-ttu-id="ee7d5-114">string</span><span class="sxs-lookup"><span data-stu-id="ee7d5-114">string</span></span> | <span data-ttu-id="ee7d5-115">A fórmula usada para calcular o valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="ee7d5-115">The formula used to compute the default value for this column.</span></span>
| <span data-ttu-id="ee7d5-116">**value**</span><span class="sxs-lookup"><span data-stu-id="ee7d5-116">**value**</span></span>     | <span data-ttu-id="ee7d5-117">string</span><span class="sxs-lookup"><span data-stu-id="ee7d5-117">string</span></span> | <span data-ttu-id="ee7d5-118">O valor direto para usar como o valor padrão dessa coluna.</span><span class="sxs-lookup"><span data-stu-id="ee7d5-118">The direct value to use as the default value for this column.</span></span>

<span data-ttu-id="ee7d5-119">Somente uma **fórmula** ou um **valor** pode ser especificado por vez.</span><span class="sxs-lookup"><span data-stu-id="ee7d5-119">Only one of **formula** or **value** may be specified at a time.</span></span>

<span data-ttu-id="ee7d5-120">As fórmulas do SharePoint usam uma sintaxe semelhante a fórmulas do Excel.</span><span class="sxs-lookup"><span data-stu-id="ee7d5-120">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="ee7d5-121">Consulte [Exemplos de fórmulas comuns em listas do SharePoint][SPFormulas] para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="ee7d5-121">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

[SPFormulas]: https://support.office.com/en-us/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DefaultColumnValue"
} -->
