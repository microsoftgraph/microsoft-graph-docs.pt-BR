---
author: JeremyKelley
description: textColumn em um recurso columnDefinition indica que os valores da coluna são texto.
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6681875328695d2e67cc10508f47183fcedb0df4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964337"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="ec776-103">Tipo de recurso TextColumn</span><span class="sxs-lookup"><span data-stu-id="ec776-103">TextColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec776-104">**textColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são texto.</span><span class="sxs-lookup"><span data-stu-id="ec776-104">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec776-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ec776-105">JSON representation</span></span>

<span data-ttu-id="ec776-106">Aqui está uma representação JSON de um recurso **textColumn**.</span><span class="sxs-lookup"><span data-stu-id="ec776-106">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="ec776-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ec776-107">Properties</span></span>

| <span data-ttu-id="ec776-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ec776-108">Property name</span></span>                   | <span data-ttu-id="ec776-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec776-109">Type</span></span>   | <span data-ttu-id="ec776-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec776-110">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="ec776-111">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="ec776-111">**allowMultipleLines**</span></span>          | <span data-ttu-id="ec776-112">string</span><span class="sxs-lookup"><span data-stu-id="ec776-112">string</span></span> | <span data-ttu-id="ec776-113">Se deseja permitir várias linhas de texto.</span><span class="sxs-lookup"><span data-stu-id="ec776-113">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="ec776-114">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="ec776-114">**appendChangesToExistingText**</span></span> | <span data-ttu-id="ec776-115">string</span><span class="sxs-lookup"><span data-stu-id="ec776-115">string</span></span> | <span data-ttu-id="ec776-116">Se as atualizações nesta coluna devem substituir o texto existente ou acrescentar a ele.</span><span class="sxs-lookup"><span data-stu-id="ec776-116">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="ec776-117">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="ec776-117">**linesForEditing**</span></span>             | <span data-ttu-id="ec776-118">int</span><span class="sxs-lookup"><span data-stu-id="ec776-118">int</span></span>    | <span data-ttu-id="ec776-119">O tamanho da caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="ec776-119">The size of the text box.</span></span>
| <span data-ttu-id="ec776-120">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="ec776-120">**maxLength**</span></span>                   | <span data-ttu-id="ec776-121">int</span><span class="sxs-lookup"><span data-stu-id="ec776-121">int</span></span>    | <span data-ttu-id="ec776-122">O número máximo de caracteres para o valor.</span><span class="sxs-lookup"><span data-stu-id="ec776-122">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="ec776-123">**textType**</span><span class="sxs-lookup"><span data-stu-id="ec776-123">**textType**</span></span>                    | <span data-ttu-id="ec776-124">string</span><span class="sxs-lookup"><span data-stu-id="ec776-124">string</span></span> | <span data-ttu-id="ec776-125">O tipo de texto sendo armazenado.</span><span class="sxs-lookup"><span data-stu-id="ec776-125">The type of text being stored.</span></span> <span data-ttu-id="ec776-126">Deve ser `plain` ou `richText`</span><span class="sxs-lookup"><span data-stu-id="ec776-126">Must be one of `plain` or `richText`</span></span>

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
