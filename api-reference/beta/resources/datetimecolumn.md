---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: DateTimeColumn
ms.openlocfilehash: 9854ad35c602ff474604f2ca88e7182c325e797d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033861"
---
# <a name="datetimecolumn-resource-type"></a><span data-ttu-id="dd1ed-102">Tipo de recurso DateTimeColumn</span><span class="sxs-lookup"><span data-stu-id="dd1ed-102">DateTimeColumn resource type</span></span>

> <span data-ttu-id="dd1ed-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dd1ed-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dd1ed-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dd1ed-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dd1ed-105">**dateTimeColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são datas ou horas.</span><span class="sxs-lookup"><span data-stu-id="dd1ed-105">The **dateTimeColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are dates or times.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd1ed-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dd1ed-106">JSON representation</span></span>

<span data-ttu-id="dd1ed-107">Aqui está uma representação JSON de um recurso **dateTimeColumn**.</span><span class="sxs-lookup"><span data-stu-id="dd1ed-107">Here is a JSON representation of a **dateTimeColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a><span data-ttu-id="dd1ed-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dd1ed-108">Properties</span></span>

| <span data-ttu-id="dd1ed-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="dd1ed-109">Property name</span></span>      | <span data-ttu-id="dd1ed-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd1ed-110">Type</span></span>               | <span data-ttu-id="dd1ed-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd1ed-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="dd1ed-112">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="dd1ed-112">**displayAs**</span></span>      | <span data-ttu-id="dd1ed-113">string</span><span class="sxs-lookup"><span data-stu-id="dd1ed-113">string</span></span>             | <span data-ttu-id="dd1ed-114">Como o valor deve ser apresentado na experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="dd1ed-114">How the value should be presented in the UX.</span></span> <span data-ttu-id="dd1ed-115">Deve ser `default`, `friendly` ou `standard`.</span><span class="sxs-lookup"><span data-stu-id="dd1ed-115">Must be one of `default`, `friendly`, or `standard`.</span></span> <span data-ttu-id="dd1ed-116">Consulte abaixo para ver mais detalhes.</span><span class="sxs-lookup"><span data-stu-id="dd1ed-116">See below for more details.</span></span> <span data-ttu-id="dd1ed-117">Se não for especificado, é tratado como `default`.</span><span class="sxs-lookup"><span data-stu-id="dd1ed-117">If unspecified, treated as `default`.</span></span>
| <span data-ttu-id="dd1ed-118">**format**</span><span class="sxs-lookup"><span data-stu-id="dd1ed-118">**format**</span></span>         | <span data-ttu-id="dd1ed-119">string</span><span class="sxs-lookup"><span data-stu-id="dd1ed-119">string</span></span>             | <span data-ttu-id="dd1ed-120">Indica se o valor deve ser apresentado como apenas uma data ou uma data e hora.</span><span class="sxs-lookup"><span data-stu-id="dd1ed-120">Indicates whether the value should be presented as a date only or a date and time.</span></span> <span data-ttu-id="dd1ed-121">Deve ser `dateOnly` ou `dateTime`</span><span class="sxs-lookup"><span data-stu-id="dd1ed-121">Must be one of `dateOnly` or `dateTime`</span></span>

## <a name="displayas-values"></a><span data-ttu-id="dd1ed-122">Valores de displayAs</span><span class="sxs-lookup"><span data-stu-id="dd1ed-122">DisplayAs values</span></span>

| <span data-ttu-id="dd1ed-123">Valor</span><span class="sxs-lookup"><span data-stu-id="dd1ed-123">Value</span></span>        | <span data-ttu-id="dd1ed-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd1ed-124">Description</span></span>
|:-------------|:--------------------------------------------------------------
| <span data-ttu-id="dd1ed-125">**default**</span><span class="sxs-lookup"><span data-stu-id="dd1ed-125">**default**</span></span>  | <span data-ttu-id="dd1ed-126">Usa o processamento de renderização padrão na UX.</span><span class="sxs-lookup"><span data-stu-id="dd1ed-126">Uses the default rendering in the UX.</span></span>
| <span data-ttu-id="dd1ed-127">**amigável**</span><span class="sxs-lookup"><span data-stu-id="dd1ed-127">**friendly**</span></span> | <span data-ttu-id="dd1ed-128">Usa uma representação amigável relativa (ex.</span><span class="sxs-lookup"><span data-stu-id="dd1ed-128">Uses a friendly relative representation (eg.</span></span> <span data-ttu-id="dd1ed-129">"hoje às 15:00")</span><span class="sxs-lookup"><span data-stu-id="dd1ed-129">"today at 3:00 PM")</span></span>
| <span data-ttu-id="dd1ed-130">**standard**</span><span class="sxs-lookup"><span data-stu-id="dd1ed-130">**standard**</span></span> | <span data-ttu-id="dd1ed-131">Usa a representação padrão absoluta (ex.</span><span class="sxs-lookup"><span data-stu-id="dd1ed-131">Uses the standard absolute representation (eg.</span></span> <span data-ttu-id="dd1ed-132">"10/05/2017 15:20")</span><span class="sxs-lookup"><span data-stu-id="dd1ed-132">"5/10/2017 3:20 PM")</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DateTimeColumn"
} -->
