---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: DateTimeColumn
localization_priority: Normal
ms.openlocfilehash: ea6298428062aa537ec25945aed339738f432762
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820843"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="96a45-102">Tipo de recurso DateTimeColumn</span><span class="sxs-lookup"><span data-stu-id="96a45-102">DateTimeColumn resource type</span></span>

<span data-ttu-id="96a45-103">**dateTimeColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são datas ou horas.</span><span class="sxs-lookup"><span data-stu-id="96a45-103">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="96a45-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="96a45-104">JSON representation</span></span>

<span data-ttu-id="96a45-105">Aqui está uma representação JSON de um recurso **dateTimeColumn**.</span><span class="sxs-lookup"><span data-stu-id="96a45-105">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="96a45-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="96a45-106">Properties</span></span>

| <span data-ttu-id="96a45-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="96a45-107">Property name</span></span>      | <span data-ttu-id="96a45-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="96a45-108">Type</span></span>               | <span data-ttu-id="96a45-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="96a45-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="96a45-110">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="96a45-110">**displayAs**</span></span>      | <span data-ttu-id="96a45-111">string</span><span class="sxs-lookup"><span data-stu-id="96a45-111">string</span></span>             | <span data-ttu-id="96a45-112">Como o valor deve ser apresentado na experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="96a45-112">How the value should be presented in the UX.</span></span> <span data-ttu-id="96a45-113">Deve ser `default`, `friendly` ou `standard`.</span><span class="sxs-lookup"><span data-stu-id="96a45-113">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="96a45-114">Consulte abaixo para ver mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="96a45-114">See below for more details.</span></span> <span data-ttu-id="96a45-115">Se não for especificado, é tratado como `default`.</span><span class="sxs-lookup"><span data-stu-id="96a45-115">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="96a45-116">**format**</span><span class="sxs-lookup"><span data-stu-id="96a45-116">**format**</span></span>         | <span data-ttu-id="96a45-117">string</span><span class="sxs-lookup"><span data-stu-id="96a45-117">string</span></span>             | <span data-ttu-id="96a45-118">Indica se o valor deve ser apresentado como apenas uma data ou uma data e hora.</span><span class="sxs-lookup"><span data-stu-id="96a45-118">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="96a45-119">Deve ser `dateOnly` ou `dateTime`</span><span class="sxs-lookup"><span data-stu-id="96a45-119">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-options"></a><span data-ttu-id="96a45-120">Opções de displayAs</span><span class="sxs-lookup"><span data-stu-id="96a45-120">DisplayAs options</span></span>

| <span data-ttu-id="96a45-121">Valor</span><span class="sxs-lookup"><span data-stu-id="96a45-121">Value</span></span>        | <span data-ttu-id="96a45-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="96a45-122">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="96a45-123">**default**</span><span class="sxs-lookup"><span data-stu-id="96a45-123">**default**</span></span>  | <span data-ttu-id="96a45-124">Usa o processamento de renderização padrão na UX.</span><span class="sxs-lookup"><span data-stu-id="96a45-124">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="96a45-125">**amigável**</span><span class="sxs-lookup"><span data-stu-id="96a45-125">**friendly**</span></span> | <span data-ttu-id="96a45-126">Usa uma representação amigável relativa (ex.</span><span class="sxs-lookup"><span data-stu-id="96a45-126">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="96a45-127">"hoje às 15:00")</span><span class="sxs-lookup"><span data-stu-id="96a45-127">"today at 3:00 PM")</span></span>
| <span data-ttu-id="96a45-128">**standard**</span><span class="sxs-lookup"><span data-stu-id="96a45-128">**standard**</span></span> | <span data-ttu-id="96a45-129">Usa a representação padrão absoluta (ex.</span><span class="sxs-lookup"><span data-stu-id="96a45-129">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="96a45-130">"10/05/2017 15:20")</span><span class="sxs-lookup"><span data-stu-id="96a45-130">"5/10/2017 3:20 PM")</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/choicecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(checkBoxes,dropDownMenu,radioButtons) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/datetimecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(default,friendly,standard) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/datetimecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(dateOnly,dateTime) are in resource, but () are in table"
  ],
  "tocPath": "Resources/DateTimeColumn"
} -->
