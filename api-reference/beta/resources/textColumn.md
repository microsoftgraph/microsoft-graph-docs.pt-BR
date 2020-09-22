---
author: JeremyKelley
description: textColumn em um recurso columnDefinition indica que os valores da coluna são texto.
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: ecfd6d72e0946519b570962577b03a9ffcbcdf10
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973544"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="13ca2-103">Tipo de recurso TextColumn</span><span class="sxs-lookup"><span data-stu-id="13ca2-103">TextColumn resource type</span></span>

<span data-ttu-id="13ca2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13ca2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13ca2-105">**textColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são texto.</span><span class="sxs-lookup"><span data-stu-id="13ca2-105">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="13ca2-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="13ca2-106">JSON representation</span></span>

<span data-ttu-id="13ca2-107">Aqui está uma representação JSON de um recurso **textColumn**.</span><span class="sxs-lookup"><span data-stu-id="13ca2-107">Here is a JSON representation of a **textColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.textColumn" } -->

```json
{
  "allowMultipleLines": true,
  "appendChangesToExistingText": false,
  "linesForEditing": 6,
  "maxLength": 300,
  "textType": "plain | richText"
}
```

## <a name="properties"></a><span data-ttu-id="13ca2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="13ca2-108">Properties</span></span>

| <span data-ttu-id="13ca2-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="13ca2-109">Property name</span></span>                   | <span data-ttu-id="13ca2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="13ca2-110">Type</span></span>   | <span data-ttu-id="13ca2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="13ca2-111">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="13ca2-112">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="13ca2-112">**allowMultipleLines**</span></span>          | <span data-ttu-id="13ca2-113">string</span><span class="sxs-lookup"><span data-stu-id="13ca2-113">string</span></span> | <span data-ttu-id="13ca2-114">Se deseja permitir várias linhas de texto.</span><span class="sxs-lookup"><span data-stu-id="13ca2-114">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="13ca2-115">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="13ca2-115">**appendChangesToExistingText**</span></span> | <span data-ttu-id="13ca2-116">string</span><span class="sxs-lookup"><span data-stu-id="13ca2-116">string</span></span> | <span data-ttu-id="13ca2-117">Se as atualizações nesta coluna devem substituir o texto existente ou acrescentar a ele.</span><span class="sxs-lookup"><span data-stu-id="13ca2-117">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="13ca2-118">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="13ca2-118">**linesForEditing**</span></span>             | <span data-ttu-id="13ca2-119">int</span><span class="sxs-lookup"><span data-stu-id="13ca2-119">int</span></span>    | <span data-ttu-id="13ca2-120">O tamanho da caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="13ca2-120">The size of the text box.</span></span>
| <span data-ttu-id="13ca2-121">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="13ca2-121">**maxLength**</span></span>                   | <span data-ttu-id="13ca2-122">int</span><span class="sxs-lookup"><span data-stu-id="13ca2-122">int</span></span>    | <span data-ttu-id="13ca2-123">O número máximo de caracteres para o valor.</span><span class="sxs-lookup"><span data-stu-id="13ca2-123">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="13ca2-124">**textType**</span><span class="sxs-lookup"><span data-stu-id="13ca2-124">**textType**</span></span>                    | <span data-ttu-id="13ca2-125">string</span><span class="sxs-lookup"><span data-stu-id="13ca2-125">string</span></span> | <span data-ttu-id="13ca2-126">O tipo de texto sendo armazenado.</span><span class="sxs-lookup"><span data-stu-id="13ca2-126">The type of text being stored.</span></span> <span data-ttu-id="13ca2-127">Deve ser `plain` ou `richText`</span><span class="sxs-lookup"><span data-stu-id="13ca2-127">Must be one of `plain` or `richText`</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn",
  "suppressions": []
}
-->


