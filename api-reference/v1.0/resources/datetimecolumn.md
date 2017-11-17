---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: DateTimeColumn
ms.openlocfilehash: ce5f06b6e0d88324813372c2431b62e6b9105bcb
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="56ef7-102">Tipo de recurso DateTimeColumn</span><span class="sxs-lookup"><span data-stu-id="56ef7-102">DateTimeColumn resource type</span></span>

<span data-ttu-id="56ef7-103">**dateTimeColumn** em um recurso [columnDefinition](columnDefinition.md) indica que os valores da coluna são datas ou horas.</span><span class="sxs-lookup"><span data-stu-id="56ef7-103">The **dateTimeColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="56ef7-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="56ef7-104">JSON representation</span></span>

<span data-ttu-id="56ef7-105">Aqui está uma representação JSON de um recurso **dateTimeColumn**.</span><span class="sxs-lookup"><span data-stu-id="56ef7-105">Here is a JSON representation of a **driveItem** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="56ef7-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="56ef7-106">Properties</span></span>

| <span data-ttu-id="56ef7-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="56ef7-107">Property name</span></span>      | <span data-ttu-id="56ef7-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="56ef7-108">Type</span></span>               | <span data-ttu-id="56ef7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="56ef7-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="56ef7-110">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="56ef7-110">**displayAs**</span></span>      | <span data-ttu-id="56ef7-111">string</span><span class="sxs-lookup"><span data-stu-id="56ef7-111">string</span></span>             | <span data-ttu-id="56ef7-112">Como o valor deve ser apresentado na experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="56ef7-112">How the value should be presented in the UX.</span></span> <span data-ttu-id="56ef7-113">Deve ser `default`, `friendly` ou `standard`.</span><span class="sxs-lookup"><span data-stu-id="56ef7-113">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="56ef7-114">Consulte abaixo para ver mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="56ef7-114">Read below for more details.</span></span> <span data-ttu-id="56ef7-115">Se não for especificado, é tratado como `default`.</span><span class="sxs-lookup"><span data-stu-id="56ef7-115">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="56ef7-116">**format**</span><span class="sxs-lookup"><span data-stu-id="56ef7-116">**format**</span></span>         | <span data-ttu-id="56ef7-117">string</span><span class="sxs-lookup"><span data-stu-id="56ef7-117">string</span></span>             | <span data-ttu-id="56ef7-118">Indica se o valor deve ser apresentado como apenas uma data ou uma data e hora.</span><span class="sxs-lookup"><span data-stu-id="56ef7-118">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="56ef7-119">Deve ser `dateOnly` ou `dateTime`</span><span class="sxs-lookup"><span data-stu-id="56ef7-119">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-values"></a><span data-ttu-id="56ef7-120">Valores de displayAs</span><span class="sxs-lookup"><span data-stu-id="56ef7-120">DisplayAs values</span></span>

| <span data-ttu-id="56ef7-121">Valor</span><span class="sxs-lookup"><span data-stu-id="56ef7-121">Value</span></span>        | <span data-ttu-id="56ef7-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="56ef7-122">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="56ef7-123">**default**</span><span class="sxs-lookup"><span data-stu-id="56ef7-123">**default**</span></span>  | <span data-ttu-id="56ef7-124">Usa o processamento de renderização padrão na UX.</span><span class="sxs-lookup"><span data-stu-id="56ef7-124">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="56ef7-125">**amigável**</span><span class="sxs-lookup"><span data-stu-id="56ef7-125">**friendly**</span></span> | <span data-ttu-id="56ef7-126">Usa uma representação amigável relativa (ex.</span><span class="sxs-lookup"><span data-stu-id="56ef7-126">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="56ef7-127">"hoje às 15:00")</span><span class="sxs-lookup"><span data-stu-id="56ef7-127">"today at 3:00 PM")</span></span>
| <span data-ttu-id="56ef7-128">**standard**</span><span class="sxs-lookup"><span data-stu-id="56ef7-128">**Standard**</span></span> | <span data-ttu-id="56ef7-129">Usa a representação padrão absoluta (ex.</span><span class="sxs-lookup"><span data-stu-id="56ef7-129">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="56ef7-130">"10/05/2017 15:20")</span><span class="sxs-lookup"><span data-stu-id="56ef7-130">"5/10/2017 3:20 PM")</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DateTimeColumn"
} -->
