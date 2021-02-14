---
author: JeremyKelley
ms.date: 09/11/2017
title: DateTimeColumn
localization_priority: Normal
description: dateTimeColumn em um recurso columnDefinition indica que os valores da coluna são datas ou horas.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 28639277416b4bcea3caf641413078e355ff9de7
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239643"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="f691d-103">Tipo de recurso DateTimeColumn</span><span class="sxs-lookup"><span data-stu-id="f691d-103">DateTimeColumn resource type</span></span>

<span data-ttu-id="f691d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f691d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f691d-105">**dateTimeColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são datas ou horas.</span><span class="sxs-lookup"><span data-stu-id="f691d-105">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f691d-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f691d-106">JSON representation</span></span>

<span data-ttu-id="f691d-107">Aqui está uma representação JSON de um recurso **dateTimeColumn**.</span><span class="sxs-lookup"><span data-stu-id="f691d-107">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="f691d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f691d-108">Properties</span></span>

| <span data-ttu-id="f691d-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="f691d-109">Property name</span></span>      | <span data-ttu-id="f691d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f691d-110">Type</span></span>               | <span data-ttu-id="f691d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f691d-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="f691d-112">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="f691d-112">**displayAs**</span></span>      | <span data-ttu-id="f691d-113">string</span><span class="sxs-lookup"><span data-stu-id="f691d-113">string</span></span>             | <span data-ttu-id="f691d-114">Como o valor deve ser apresentado na experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="f691d-114">How the value should be presented in the UX.</span></span> <span data-ttu-id="f691d-115">Deve ser `default`, `friendly` ou `standard`.</span><span class="sxs-lookup"><span data-stu-id="f691d-115">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="f691d-116">Consulte abaixo para ver mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="f691d-116">See below for more details.</span></span> <span data-ttu-id="f691d-117">Se não for especificado, é tratado como `default`.</span><span class="sxs-lookup"><span data-stu-id="f691d-117">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="f691d-118">**format**</span><span class="sxs-lookup"><span data-stu-id="f691d-118">**format**</span></span>         | <span data-ttu-id="f691d-119">string</span><span class="sxs-lookup"><span data-stu-id="f691d-119">string</span></span>             | <span data-ttu-id="f691d-120">Indica se o valor deve ser apresentado como apenas uma data ou uma data e hora.</span><span class="sxs-lookup"><span data-stu-id="f691d-120">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="f691d-121">Deve ser `dateOnly` ou `dateTime`</span><span class="sxs-lookup"><span data-stu-id="f691d-121">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-options"></a><span data-ttu-id="f691d-122">Opções de DisplayAs</span><span class="sxs-lookup"><span data-stu-id="f691d-122">DisplayAs options</span></span>

| <span data-ttu-id="f691d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="f691d-123">Value</span></span>        | <span data-ttu-id="f691d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f691d-124">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="f691d-125">**default**</span><span class="sxs-lookup"><span data-stu-id="f691d-125">**default**</span></span>  | <span data-ttu-id="f691d-126">Usa o processamento de renderização padrão na UX.</span><span class="sxs-lookup"><span data-stu-id="f691d-126">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="f691d-127">**amigável**</span><span class="sxs-lookup"><span data-stu-id="f691d-127">**friendly**</span></span> | <span data-ttu-id="f691d-128">Usa uma representação amigável relativa (ex.</span><span class="sxs-lookup"><span data-stu-id="f691d-128">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="f691d-129">"hoje às 15:00")</span><span class="sxs-lookup"><span data-stu-id="f691d-129">"today at 3:00 PM")</span></span>
| <span data-ttu-id="f691d-130">**standard**</span><span class="sxs-lookup"><span data-stu-id="f691d-130">**standard**</span></span> | <span data-ttu-id="f691d-131">Usa a representação padrão absoluta (ex.</span><span class="sxs-lookup"><span data-stu-id="f691d-131">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="f691d-132">"10/05/2017 15:20")</span><span class="sxs-lookup"><span data-stu-id="f691d-132">"5/10/2017 3:20 PM")</span></span>


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

