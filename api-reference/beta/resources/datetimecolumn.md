---
author: JeremyKelley
description: dateTimeColumn em um recurso columnDefinition indica que os valores da coluna são datas ou horas.
ms.date: 09/11/2017
title: DateTimeColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e0e69e4019530031966cde9f782c2f017ba976fb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973881"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="b564a-103">Tipo de recurso DateTimeColumn</span><span class="sxs-lookup"><span data-stu-id="b564a-103">DateTimeColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b564a-104">**dateTimeColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são datas ou horas.</span><span class="sxs-lookup"><span data-stu-id="b564a-104">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b564a-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b564a-105">JSON representation</span></span>

<span data-ttu-id="b564a-106">Aqui está uma representação JSON de um recurso **dateTimeColumn**.</span><span class="sxs-lookup"><span data-stu-id="b564a-106">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="b564a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b564a-107">Properties</span></span>

| <span data-ttu-id="b564a-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="b564a-108">Property name</span></span>      | <span data-ttu-id="b564a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b564a-109">Type</span></span>               | <span data-ttu-id="b564a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b564a-110">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="b564a-111">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="b564a-111">**displayAs**</span></span>      | <span data-ttu-id="b564a-112">string</span><span class="sxs-lookup"><span data-stu-id="b564a-112">string</span></span>             | <span data-ttu-id="b564a-113">Como o valor deve ser apresentado na experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="b564a-113">How the value should be presented in the UX.</span></span> <span data-ttu-id="b564a-114">Deve ser `default`, `friendly` ou `standard`.</span><span class="sxs-lookup"><span data-stu-id="b564a-114">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="b564a-115">Consulte abaixo para ver mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="b564a-115">See below for more details.</span></span> <span data-ttu-id="b564a-116">Se não for especificado, é tratado como `default`.</span><span class="sxs-lookup"><span data-stu-id="b564a-116">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="b564a-117">**format**</span><span class="sxs-lookup"><span data-stu-id="b564a-117">**format**</span></span>         | <span data-ttu-id="b564a-118">string</span><span class="sxs-lookup"><span data-stu-id="b564a-118">string</span></span>             | <span data-ttu-id="b564a-119">Indica se o valor deve ser apresentado como apenas uma data ou uma data e hora.</span><span class="sxs-lookup"><span data-stu-id="b564a-119">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="b564a-120">Deve ser `dateOnly` ou `dateTime`</span><span class="sxs-lookup"><span data-stu-id="b564a-120">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-values"></a><span data-ttu-id="b564a-121">Valores de displayAs</span><span class="sxs-lookup"><span data-stu-id="b564a-121">DisplayAs values</span></span>

| <span data-ttu-id="b564a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b564a-122">Value</span></span>        | <span data-ttu-id="b564a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b564a-123">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="b564a-124">**default**</span><span class="sxs-lookup"><span data-stu-id="b564a-124">**default**</span></span>  | <span data-ttu-id="b564a-125">Usa o processamento de renderização padrão na UX.</span><span class="sxs-lookup"><span data-stu-id="b564a-125">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="b564a-126">**amigável**</span><span class="sxs-lookup"><span data-stu-id="b564a-126">**friendly**</span></span> | <span data-ttu-id="b564a-127">Usa uma representação amigável relativa (ex.</span><span class="sxs-lookup"><span data-stu-id="b564a-127">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="b564a-128">"hoje às 15:00")</span><span class="sxs-lookup"><span data-stu-id="b564a-128">"today at 3:00 PM")</span></span>
| <span data-ttu-id="b564a-129">**standard**</span><span class="sxs-lookup"><span data-stu-id="b564a-129">**standard**</span></span> | <span data-ttu-id="b564a-130">Usa a representação padrão absoluta (ex.</span><span class="sxs-lookup"><span data-stu-id="b564a-130">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="b564a-131">"10/05/2017 15:20")</span><span class="sxs-lookup"><span data-stu-id="b564a-131">"5/10/2017 3:20 PM")</span></span>


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
