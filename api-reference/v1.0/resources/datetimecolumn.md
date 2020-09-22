---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: DateTimeColumn
localization_priority: Normal
description: dateTimeColumn em um recurso columnDefinition indica que os valores da coluna são datas ou horas.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 37ae27f2ae9b74612895784e69752d37ef976b04
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091835"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="d0838-103">Tipo de recurso DateTimeColumn</span><span class="sxs-lookup"><span data-stu-id="d0838-103">DateTimeColumn resource type</span></span>

<span data-ttu-id="d0838-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0838-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d0838-105">**dateTimeColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são datas ou horas.</span><span class="sxs-lookup"><span data-stu-id="d0838-105">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0838-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d0838-106">JSON representation</span></span>

<span data-ttu-id="d0838-107">Aqui está uma representação JSON de um recurso **dateTimeColumn**.</span><span class="sxs-lookup"><span data-stu-id="d0838-107">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="d0838-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d0838-108">Properties</span></span>

| <span data-ttu-id="d0838-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="d0838-109">Property name</span></span>      | <span data-ttu-id="d0838-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0838-110">Type</span></span>               | <span data-ttu-id="d0838-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0838-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="d0838-112">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="d0838-112">**displayAs**</span></span>      | <span data-ttu-id="d0838-113">string</span><span class="sxs-lookup"><span data-stu-id="d0838-113">string</span></span>             | <span data-ttu-id="d0838-114">Como o valor deve ser apresentado na experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="d0838-114">How the value should be presented in the UX.</span></span> <span data-ttu-id="d0838-115">Deve ser `default`, `friendly` ou `standard`.</span><span class="sxs-lookup"><span data-stu-id="d0838-115">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="d0838-116">Consulte abaixo para ver mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="d0838-116">See below for more details.</span></span> <span data-ttu-id="d0838-117">Se não for especificado, é tratado como `default`.</span><span class="sxs-lookup"><span data-stu-id="d0838-117">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="d0838-118">**format**</span><span class="sxs-lookup"><span data-stu-id="d0838-118">**format**</span></span>         | <span data-ttu-id="d0838-119">string</span><span class="sxs-lookup"><span data-stu-id="d0838-119">string</span></span>             | <span data-ttu-id="d0838-120">Indica se o valor deve ser apresentado como apenas uma data ou uma data e hora.</span><span class="sxs-lookup"><span data-stu-id="d0838-120">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="d0838-121">Deve ser `dateOnly` ou `dateTime`</span><span class="sxs-lookup"><span data-stu-id="d0838-121">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-options"></a><span data-ttu-id="d0838-122">Opções de displayas</span><span class="sxs-lookup"><span data-stu-id="d0838-122">DisplayAs options</span></span>

| <span data-ttu-id="d0838-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d0838-123">Value</span></span>        | <span data-ttu-id="d0838-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0838-124">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="d0838-125">**default**</span><span class="sxs-lookup"><span data-stu-id="d0838-125">**default**</span></span>  | <span data-ttu-id="d0838-126">Usa o processamento de renderização padrão na UX.</span><span class="sxs-lookup"><span data-stu-id="d0838-126">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="d0838-127">**amigável**</span><span class="sxs-lookup"><span data-stu-id="d0838-127">**friendly**</span></span> | <span data-ttu-id="d0838-128">Usa uma representação amigável relativa (ex.</span><span class="sxs-lookup"><span data-stu-id="d0838-128">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="d0838-129">"hoje às 15:00")</span><span class="sxs-lookup"><span data-stu-id="d0838-129">"today at 3:00 PM")</span></span>
| <span data-ttu-id="d0838-130">**standard**</span><span class="sxs-lookup"><span data-stu-id="d0838-130">**standard**</span></span> | <span data-ttu-id="d0838-131">Usa a representação padrão absoluta (ex.</span><span class="sxs-lookup"><span data-stu-id="d0838-131">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="d0838-132">"10/05/2017 15:20")</span><span class="sxs-lookup"><span data-stu-id="d0838-132">"5/10/2017 3:20 PM")</span></span>


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

