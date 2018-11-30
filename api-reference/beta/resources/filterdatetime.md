---
title: Tipo de recurso FilterDatetime
description: Indica como filtrar uma data ao filtrar valores.
ms.openlocfilehash: d3cb0df48a1116a64a72413aa64cabdec46da6d9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037333"
---
# <a name="filterdatetime-resource-type"></a><span data-ttu-id="66d09-103">Tipo de recurso FilterDatetime</span><span class="sxs-lookup"><span data-stu-id="66d09-103">FilterDatetime resource type</span></span>

> <span data-ttu-id="66d09-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="66d09-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66d09-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="66d09-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="66d09-106">Indica como filtrar uma data ao filtrar valores.</span><span class="sxs-lookup"><span data-stu-id="66d09-106">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="66d09-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="66d09-107">Properties</span></span>
| <span data-ttu-id="66d09-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="66d09-108">Property</span></span>     | <span data-ttu-id="66d09-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="66d09-109">Type</span></span>   |<span data-ttu-id="66d09-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="66d09-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66d09-111">data</span><span class="sxs-lookup"><span data-stu-id="66d09-111">date</span></span>|<span data-ttu-id="66d09-112">string</span><span class="sxs-lookup"><span data-stu-id="66d09-112">string</span></span>|<span data-ttu-id="66d09-113">A data no formato ISO8601 usada para filtrar os dados.</span><span class="sxs-lookup"><span data-stu-id="66d09-113">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="66d09-114">especificidade</span><span class="sxs-lookup"><span data-stu-id="66d09-114">specificity</span></span>|<span data-ttu-id="66d09-115">string</span><span class="sxs-lookup"><span data-stu-id="66d09-115">string</span></span>|<span data-ttu-id="66d09-p102">Como a data específica deve ser usada para manter os dados. Por exemplo, se a data for 2005-04-02 e a especificidade estiver definida como "mês", a operação de filtragem manterá todas as linhas com uma data do mês de abril de 2009. Os valores possíveis são: `Year`, `Monday`, `Day`, `Hour`, `Minute` e `Second`.</span><span class="sxs-lookup"><span data-stu-id="66d09-p102">How specific the date should be used to keep data. For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009. Possible values are: `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66d09-119">Relações</span><span class="sxs-lookup"><span data-stu-id="66d09-119">Relationships</span></span>
<span data-ttu-id="66d09-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="66d09-120">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="66d09-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="66d09-121">JSON representation</span></span>

<span data-ttu-id="66d09-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="66d09-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterDateTime"
}-->

```json
{
  "date": "string",
  "specificity": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->