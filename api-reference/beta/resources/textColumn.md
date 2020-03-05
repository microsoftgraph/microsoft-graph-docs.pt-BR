---
author: JeremyKelley
description: textColumn em um recurso columnDefinition indica que os valores da coluna são texto.
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e6167a81c0898b2de1c5878926633f8dbd0baa2d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519789"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="77901-103">Tipo de recurso TextColumn</span><span class="sxs-lookup"><span data-stu-id="77901-103">TextColumn resource type</span></span>

<span data-ttu-id="77901-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="77901-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77901-105">**textColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são texto.</span><span class="sxs-lookup"><span data-stu-id="77901-105">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="77901-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="77901-106">JSON representation</span></span>

<span data-ttu-id="77901-107">Aqui está uma representação JSON de um recurso **textColumn**.</span><span class="sxs-lookup"><span data-stu-id="77901-107">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="77901-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="77901-108">Properties</span></span>

| <span data-ttu-id="77901-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="77901-109">Property name</span></span>                   | <span data-ttu-id="77901-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="77901-110">Type</span></span>   | <span data-ttu-id="77901-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="77901-111">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="77901-112">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="77901-112">**allowMultipleLines**</span></span>          | <span data-ttu-id="77901-113">string</span><span class="sxs-lookup"><span data-stu-id="77901-113">string</span></span> | <span data-ttu-id="77901-114">Se deseja permitir várias linhas de texto.</span><span class="sxs-lookup"><span data-stu-id="77901-114">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="77901-115">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="77901-115">**appendChangesToExistingText**</span></span> | <span data-ttu-id="77901-116">string</span><span class="sxs-lookup"><span data-stu-id="77901-116">string</span></span> | <span data-ttu-id="77901-117">Se as atualizações nesta coluna devem substituir o texto existente ou acrescentar a ele.</span><span class="sxs-lookup"><span data-stu-id="77901-117">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="77901-118">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="77901-118">**linesForEditing**</span></span>             | <span data-ttu-id="77901-119">int</span><span class="sxs-lookup"><span data-stu-id="77901-119">int</span></span>    | <span data-ttu-id="77901-120">O tamanho da caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="77901-120">The size of the text box.</span></span>
| <span data-ttu-id="77901-121">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="77901-121">**maxLength**</span></span>                   | <span data-ttu-id="77901-122">int</span><span class="sxs-lookup"><span data-stu-id="77901-122">int</span></span>    | <span data-ttu-id="77901-123">O número máximo de caracteres para o valor.</span><span class="sxs-lookup"><span data-stu-id="77901-123">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="77901-124">**textType**</span><span class="sxs-lookup"><span data-stu-id="77901-124">**textType**</span></span>                    | <span data-ttu-id="77901-125">string</span><span class="sxs-lookup"><span data-stu-id="77901-125">string</span></span> | <span data-ttu-id="77901-126">O tipo de texto sendo armazenado.</span><span class="sxs-lookup"><span data-stu-id="77901-126">The type of text being stored.</span></span> <span data-ttu-id="77901-127">Deve ser `plain` ou `richText`</span><span class="sxs-lookup"><span data-stu-id="77901-127">Must be one of `plain` or `richText`</span></span>

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
