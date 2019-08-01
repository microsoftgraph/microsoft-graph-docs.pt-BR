---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
description: textColumn em um recurso columnDefinition indica que os valores da coluna são texto.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 37a5bbd985d163cf627f4bc0a16a756eaf00af66
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033653"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="029e1-103">Tipo de recurso TextColumn</span><span class="sxs-lookup"><span data-stu-id="029e1-103">TextColumn resource type</span></span>

<span data-ttu-id="029e1-104">**textColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são texto.</span><span class="sxs-lookup"><span data-stu-id="029e1-104">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="029e1-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="029e1-105">JSON representation</span></span>

<span data-ttu-id="029e1-106">Aqui está uma representação JSON de um recurso **textColumn**.</span><span class="sxs-lookup"><span data-stu-id="029e1-106">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="029e1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="029e1-107">Properties</span></span>

| <span data-ttu-id="029e1-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="029e1-108">Property name</span></span>                   | <span data-ttu-id="029e1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="029e1-109">Type</span></span>    | <span data-ttu-id="029e1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="029e1-110">Description</span></span>
|:--------------------------------|:--------|:---------------------------------
| <span data-ttu-id="029e1-111">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="029e1-111">**allowMultipleLines**</span></span>          | <span data-ttu-id="029e1-112">booliano</span><span class="sxs-lookup"><span data-stu-id="029e1-112">boolean</span></span> | <span data-ttu-id="029e1-113">Se deseja permitir várias linhas de texto.</span><span class="sxs-lookup"><span data-stu-id="029e1-113">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="029e1-114">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="029e1-114">**appendChangesToExistingText**</span></span> | <span data-ttu-id="029e1-115">booliano</span><span class="sxs-lookup"><span data-stu-id="029e1-115">boolean</span></span> | <span data-ttu-id="029e1-116">Se as atualizações nesta coluna devem substituir o texto existente ou acrescentar a ele.</span><span class="sxs-lookup"><span data-stu-id="029e1-116">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="029e1-117">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="029e1-117">**linesForEditing**</span></span>             | <span data-ttu-id="029e1-118">int32</span><span class="sxs-lookup"><span data-stu-id="029e1-118">int32</span></span>   | <span data-ttu-id="029e1-119">O tamanho da caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="029e1-119">The size of the text box.</span></span>
| <span data-ttu-id="029e1-120">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="029e1-120">**maxLength**</span></span>                   | <span data-ttu-id="029e1-121">int32</span><span class="sxs-lookup"><span data-stu-id="029e1-121">int32</span></span>   | <span data-ttu-id="029e1-122">O número máximo de caracteres para o valor.</span><span class="sxs-lookup"><span data-stu-id="029e1-122">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="029e1-123">**textType**</span><span class="sxs-lookup"><span data-stu-id="029e1-123">**textType**</span></span>                    | <span data-ttu-id="029e1-124">string</span><span class="sxs-lookup"><span data-stu-id="029e1-124">string</span></span>  | <span data-ttu-id="029e1-125">O tipo de texto sendo armazenado.</span><span class="sxs-lookup"><span data-stu-id="029e1-125">The type of text being stored.</span></span> <span data-ttu-id="029e1-126">Deve ser `plain` ou `richText`</span><span class="sxs-lookup"><span data-stu-id="029e1-126">Must be one of `plain` or `richText`</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/textcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(plain,richText) are in resource, but () are in table"
  ],
  "tocPath": "Resources/TextColumn"
} -->
