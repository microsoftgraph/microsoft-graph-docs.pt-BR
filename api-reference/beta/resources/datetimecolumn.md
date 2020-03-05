---
author: JeremyKelley
description: dateTimeColumn em um recurso columnDefinition indica que os valores da coluna são datas ou horas.
ms.date: 09/11/2017
title: DateTimeColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 5c2a90a67a8a283dbc1da497c5824e4eb7ecbc85
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507300"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="9634f-103">Tipo de recurso DateTimeColumn</span><span class="sxs-lookup"><span data-stu-id="9634f-103">DateTimeColumn resource type</span></span>

<span data-ttu-id="9634f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9634f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9634f-105">**dateTimeColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são datas ou horas.</span><span class="sxs-lookup"><span data-stu-id="9634f-105">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9634f-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9634f-106">JSON representation</span></span>

<span data-ttu-id="9634f-107">Aqui está uma representação JSON de um recurso **dateTimeColumn**.</span><span class="sxs-lookup"><span data-stu-id="9634f-107">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="9634f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9634f-108">Properties</span></span>

| <span data-ttu-id="9634f-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="9634f-109">Property name</span></span>      | <span data-ttu-id="9634f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9634f-110">Type</span></span>               | <span data-ttu-id="9634f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9634f-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="9634f-112">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="9634f-112">**displayAs**</span></span>      | <span data-ttu-id="9634f-113">string</span><span class="sxs-lookup"><span data-stu-id="9634f-113">string</span></span>             | <span data-ttu-id="9634f-114">Como o valor deve ser apresentado na experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="9634f-114">How the value should be presented in the UX.</span></span> <span data-ttu-id="9634f-115">Deve ser `default`, `friendly` ou `standard`.</span><span class="sxs-lookup"><span data-stu-id="9634f-115">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="9634f-116">Consulte abaixo para ver mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="9634f-116">See below for more details.</span></span> <span data-ttu-id="9634f-117">Se não for especificado, é tratado como `default`.</span><span class="sxs-lookup"><span data-stu-id="9634f-117">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="9634f-118">**format**</span><span class="sxs-lookup"><span data-stu-id="9634f-118">**format**</span></span>         | <span data-ttu-id="9634f-119">string</span><span class="sxs-lookup"><span data-stu-id="9634f-119">string</span></span>             | <span data-ttu-id="9634f-120">Indica se o valor deve ser apresentado como apenas uma data ou uma data e hora.</span><span class="sxs-lookup"><span data-stu-id="9634f-120">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="9634f-121">Deve ser `dateOnly` ou `dateTime`</span><span class="sxs-lookup"><span data-stu-id="9634f-121">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-values"></a><span data-ttu-id="9634f-122">Valores de displayAs</span><span class="sxs-lookup"><span data-stu-id="9634f-122">DisplayAs values</span></span>

| <span data-ttu-id="9634f-123">Valor</span><span class="sxs-lookup"><span data-stu-id="9634f-123">Value</span></span>        | <span data-ttu-id="9634f-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9634f-124">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="9634f-125">**default**</span><span class="sxs-lookup"><span data-stu-id="9634f-125">**default**</span></span>  | <span data-ttu-id="9634f-126">Usa o processamento de renderização padrão na UX.</span><span class="sxs-lookup"><span data-stu-id="9634f-126">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="9634f-127">**amigável**</span><span class="sxs-lookup"><span data-stu-id="9634f-127">**friendly**</span></span> | <span data-ttu-id="9634f-128">Usa uma representação amigável relativa (ex.</span><span class="sxs-lookup"><span data-stu-id="9634f-128">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="9634f-129">"hoje às 15:00")</span><span class="sxs-lookup"><span data-stu-id="9634f-129">"today at 3:00 PM")</span></span>
| <span data-ttu-id="9634f-130">**standard**</span><span class="sxs-lookup"><span data-stu-id="9634f-130">**standard**</span></span> | <span data-ttu-id="9634f-131">Usa a representação padrão absoluta (ex.</span><span class="sxs-lookup"><span data-stu-id="9634f-131">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="9634f-132">"10/05/2017 15:20")</span><span class="sxs-lookup"><span data-stu-id="9634f-132">"5/10/2017 3:20 PM")</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DateTimeColumn",
  "suppressions": []
}
-->
