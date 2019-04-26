---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: DateTimeColumn
localization_priority: Normal
ms.openlocfilehash: b80e4a2e156baae4fbd8f3b559f061c50b45505f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340970"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="b2cca-102">Tipo de recurso DateTimeColumn</span><span class="sxs-lookup"><span data-stu-id="b2cca-102">DateTimeColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2cca-103">**dateTimeColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são datas ou horas.</span><span class="sxs-lookup"><span data-stu-id="b2cca-103">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2cca-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b2cca-104">JSON representation</span></span>

<span data-ttu-id="b2cca-105">Aqui está uma representação JSON de um recurso **dateTimeColumn**.</span><span class="sxs-lookup"><span data-stu-id="b2cca-105">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="b2cca-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b2cca-106">Properties</span></span>

| <span data-ttu-id="b2cca-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="b2cca-107">Property name</span></span>      | <span data-ttu-id="b2cca-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b2cca-108">Type</span></span>               | <span data-ttu-id="b2cca-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2cca-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="b2cca-110">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="b2cca-110">**displayAs**</span></span>      | <span data-ttu-id="b2cca-111">string</span><span class="sxs-lookup"><span data-stu-id="b2cca-111">string</span></span>             | <span data-ttu-id="b2cca-112">Como o valor deve ser apresentado na experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="b2cca-112">How the value should be presented in the UX.</span></span> <span data-ttu-id="b2cca-113">Deve ser `default`, `friendly` ou `standard`.</span><span class="sxs-lookup"><span data-stu-id="b2cca-113">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="b2cca-114">Consulte abaixo para ver mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="b2cca-114">See below for more details.</span></span> <span data-ttu-id="b2cca-115">Se não for especificado, é tratado como `default`.</span><span class="sxs-lookup"><span data-stu-id="b2cca-115">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="b2cca-116">**format**</span><span class="sxs-lookup"><span data-stu-id="b2cca-116">**format**</span></span>         | <span data-ttu-id="b2cca-117">string</span><span class="sxs-lookup"><span data-stu-id="b2cca-117">string</span></span>             | <span data-ttu-id="b2cca-118">Indica se o valor deve ser apresentado como apenas uma data ou uma data e hora.</span><span class="sxs-lookup"><span data-stu-id="b2cca-118">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="b2cca-119">Deve ser `dateOnly` ou `dateTime`</span><span class="sxs-lookup"><span data-stu-id="b2cca-119">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-values"></a><span data-ttu-id="b2cca-120">Valores de displayAs</span><span class="sxs-lookup"><span data-stu-id="b2cca-120">DisplayAs values</span></span>

| <span data-ttu-id="b2cca-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b2cca-121">Value</span></span>        | <span data-ttu-id="b2cca-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2cca-122">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="b2cca-123">**default**</span><span class="sxs-lookup"><span data-stu-id="b2cca-123">**default**</span></span>  | <span data-ttu-id="b2cca-124">Usa o processamento de renderização padrão na UX.</span><span class="sxs-lookup"><span data-stu-id="b2cca-124">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="b2cca-125">**amigável**</span><span class="sxs-lookup"><span data-stu-id="b2cca-125">**friendly**</span></span> | <span data-ttu-id="b2cca-126">Usa uma representação amigável relativa (ex.</span><span class="sxs-lookup"><span data-stu-id="b2cca-126">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="b2cca-127">"hoje às 15:00")</span><span class="sxs-lookup"><span data-stu-id="b2cca-127">"today at 3:00 PM")</span></span>
| <span data-ttu-id="b2cca-128">**standard**</span><span class="sxs-lookup"><span data-stu-id="b2cca-128">**standard**</span></span> | <span data-ttu-id="b2cca-129">Usa a representação padrão absoluta (ex.</span><span class="sxs-lookup"><span data-stu-id="b2cca-129">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="b2cca-130">"10/05/2017 15:20")</span><span class="sxs-lookup"><span data-stu-id="b2cca-130">"5/10/2017 3:20 PM")</span></span>


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
