---
author: swapnil1993
title: tipo de recurso columnValidation
description: Contém dados para validar valores de coluna.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: 8c1b20b239b894aa0da63222bb69a8d720e5ab50
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445929"
---
# <a name="columnvalidation-resource-type"></a><span data-ttu-id="a3f5f-103">tipo de recurso columnValidation</span><span class="sxs-lookup"><span data-stu-id="a3f5f-103">columnValidation resource type</span></span>

<span data-ttu-id="a3f5f-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span><span class="sxs-lookup"><span data-stu-id="a3f5f-104">Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]</span></span>
<span data-ttu-id="a3f5f-105">Contém metadados para validar a coluna.</span><span class="sxs-lookup"><span data-stu-id="a3f5f-105">Contains metadata for validating the column.</span></span>


## <a name="properties"></a><span data-ttu-id="a3f5f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a3f5f-106">Properties</span></span>

| <span data-ttu-id="a3f5f-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="a3f5f-107">Property name</span></span>  | <span data-ttu-id="a3f5f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3f5f-108">Type</span></span>    | <span data-ttu-id="a3f5f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3f5f-109">Description</span></span>
|:---------------|:--------|:--------------------------------------------------
| <span data-ttu-id="a3f5f-110">**formula**</span><span class="sxs-lookup"><span data-stu-id="a3f5f-110">**formula**</span></span>    | <span data-ttu-id="a3f5f-111">string</span><span class="sxs-lookup"><span data-stu-id="a3f5f-111">string</span></span>  | <span data-ttu-id="a3f5f-112">A fórmula para validar o valor da coluna.</span><span class="sxs-lookup"><span data-stu-id="a3f5f-112">The formula to validate column value.</span></span> <span data-ttu-id="a3f5f-113">Por exemplos, consulte [Exemplos de fórmulas comuns em listas](https://support.microsoft.com/office/examples-of-common-formulas-in-sharepoint-lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3)</span><span class="sxs-lookup"><span data-stu-id="a3f5f-113">For examples, see [Examples of common formulas in lists](https://support.microsoft.com/office/examples-of-common-formulas-in-sharepoint-lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3)</span></span> 
| <span data-ttu-id="a3f5f-114">**descriptions**</span><span class="sxs-lookup"><span data-stu-id="a3f5f-114">**descriptions**</span></span>    | <span data-ttu-id="a3f5f-115">Collection(microsoft.graph.displayNameLocalization)</span><span class="sxs-lookup"><span data-stu-id="a3f5f-115">Collection(microsoft.graph.displayNameLocalization)</span></span>  | <span data-ttu-id="a3f5f-116">Mensagens localizadas que explicam o que é necessário para que o valor dessa coluna seja considerado válido.</span><span class="sxs-lookup"><span data-stu-id="a3f5f-116">Localized messages that explain what is needed for this column's value to be considered valid.</span></span> <span data-ttu-id="a3f5f-117">O usuário será solicitado com essa mensagem se a validação falhar.</span><span class="sxs-lookup"><span data-stu-id="a3f5f-117">User will be prompted with this message if validation fails.</span></span> 
| <span data-ttu-id="a3f5f-118">**defaultLanguage**</span><span class="sxs-lookup"><span data-stu-id="a3f5f-118">**defaultLanguage**</span></span>    | <span data-ttu-id="a3f5f-119">string</span><span class="sxs-lookup"><span data-stu-id="a3f5f-119">string</span></span>  | <span data-ttu-id="a3f5f-120">Marca de idioma padrão BCP 47 para a descrição.</span><span class="sxs-lookup"><span data-stu-id="a3f5f-120">Default BCP 47 language tag for the description.</span></span>

<span data-ttu-id="a3f5f-121">As fórmulas do SharePoint usam uma sintaxe semelhante a fórmulas do Excel.</span><span class="sxs-lookup"><span data-stu-id="a3f5f-121">SharePoint formulas use a syntax similar to Excel formulas.</span></span>
<span data-ttu-id="a3f5f-122">Consulte [Exemplos de fórmulas comuns em listas do SharePoint][SPFormulas] para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="a3f5f-122">See [Examples of common formulas in SharePoint Lists][SPFormulas] for more information.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3f5f-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a3f5f-123">JSON representation</span></span>

<span data-ttu-id="a3f5f-124">A seguir está uma representação JSON de um **recurso columnValidation.**</span><span class="sxs-lookup"><span data-stu-id="a3f5f-124">The following is a JSON representation of a **columnValidation** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnValidation"} -->

```json
{
  "formula": "string",
  "descriptions": [{ "@type": "microsoft.graph.displayNameLocalization" }],
  "defaultLanguage": "string"
}
```

[SPFormulas]: https://support.office.com/article/Examples-of-common-formulas-in-SharePoint-Lists-d81f5f21-2b4e-45ce-b170-bf7ebf6988b3
