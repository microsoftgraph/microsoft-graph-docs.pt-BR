---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: DateTimeColumn
localization_priority: Normal
ms.openlocfilehash: 03ebb78adda52a9f98aec6635bbda48dd61e37e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889212"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="cd6eb-102">Tipo de recurso DateTimeColumn</span><span class="sxs-lookup"><span data-stu-id="cd6eb-102">DateTimeColumn resource type</span></span>

> <span data-ttu-id="cd6eb-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cd6eb-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd6eb-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cd6eb-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd6eb-105">**dateTimeColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são datas ou horas.</span><span class="sxs-lookup"><span data-stu-id="cd6eb-105">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd6eb-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cd6eb-106">JSON representation</span></span>

<span data-ttu-id="cd6eb-107">Aqui está uma representação JSON de um recurso **dateTimeColumn**.</span><span class="sxs-lookup"><span data-stu-id="cd6eb-107">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="cd6eb-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cd6eb-108">Properties</span></span>

| <span data-ttu-id="cd6eb-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="cd6eb-109">Property name</span></span>      | <span data-ttu-id="cd6eb-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd6eb-110">Type</span></span>               | <span data-ttu-id="cd6eb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd6eb-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="cd6eb-112">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="cd6eb-112">**displayAs**</span></span>      | <span data-ttu-id="cd6eb-113">string</span><span class="sxs-lookup"><span data-stu-id="cd6eb-113">string</span></span>             | <span data-ttu-id="cd6eb-114">Como o valor deve ser apresentado na experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="cd6eb-114">How the value should be presented in the UX.</span></span> <span data-ttu-id="cd6eb-115">Deve ser `default`, `friendly` ou `standard`.</span><span class="sxs-lookup"><span data-stu-id="cd6eb-115">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="cd6eb-116">Consulte abaixo para ver mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="cd6eb-116">See below for more details.</span></span> <span data-ttu-id="cd6eb-117">Se não for especificado, é tratado como `default`.</span><span class="sxs-lookup"><span data-stu-id="cd6eb-117">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="cd6eb-118">**format**</span><span class="sxs-lookup"><span data-stu-id="cd6eb-118">**format**</span></span>         | <span data-ttu-id="cd6eb-119">string</span><span class="sxs-lookup"><span data-stu-id="cd6eb-119">string</span></span>             | <span data-ttu-id="cd6eb-120">Indica se o valor deve ser apresentado como apenas uma data ou uma data e hora.</span><span class="sxs-lookup"><span data-stu-id="cd6eb-120">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="cd6eb-121">Deve ser `dateOnly` ou `dateTime`</span><span class="sxs-lookup"><span data-stu-id="cd6eb-121">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-values"></a><span data-ttu-id="cd6eb-122">Valores de displayAs</span><span class="sxs-lookup"><span data-stu-id="cd6eb-122">DisplayAs values</span></span>

| <span data-ttu-id="cd6eb-123">Valor</span><span class="sxs-lookup"><span data-stu-id="cd6eb-123">Value</span></span>        | <span data-ttu-id="cd6eb-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd6eb-124">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="cd6eb-125">**default**</span><span class="sxs-lookup"><span data-stu-id="cd6eb-125">**default**</span></span>  | <span data-ttu-id="cd6eb-126">Usa o processamento de renderização padrão na UX.</span><span class="sxs-lookup"><span data-stu-id="cd6eb-126">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="cd6eb-127">**amigável**</span><span class="sxs-lookup"><span data-stu-id="cd6eb-127">**friendly**</span></span> | <span data-ttu-id="cd6eb-128">Usa uma representação amigável relativa (ex.</span><span class="sxs-lookup"><span data-stu-id="cd6eb-128">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="cd6eb-129">"hoje às 15:00")</span><span class="sxs-lookup"><span data-stu-id="cd6eb-129">"today at 3:00 PM")</span></span>
| <span data-ttu-id="cd6eb-130">**standard**</span><span class="sxs-lookup"><span data-stu-id="cd6eb-130">**standard**</span></span> | <span data-ttu-id="cd6eb-131">Usa a representação padrão absoluta (ex.</span><span class="sxs-lookup"><span data-stu-id="cd6eb-131">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="cd6eb-132">"10/05/2017 15:20")</span><span class="sxs-lookup"><span data-stu-id="cd6eb-132">"5/10/2017 3:20 PM")</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DateTimeColumn"
} -->
