---
author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
description: textColumn em um recurso columnDefinition indica que os valores da coluna são texto.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 62711f2f44004e5b3d594eb472b7c018205d9e31
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239271"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="499be-103">Tipo de recurso TextColumn</span><span class="sxs-lookup"><span data-stu-id="499be-103">TextColumn resource type</span></span>

<span data-ttu-id="499be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="499be-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="499be-105">**textColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são texto.</span><span class="sxs-lookup"><span data-stu-id="499be-105">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="499be-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="499be-106">JSON representation</span></span>

<span data-ttu-id="499be-107">Aqui está uma representação JSON de um recurso **textColumn**.</span><span class="sxs-lookup"><span data-stu-id="499be-107">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="499be-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="499be-108">Properties</span></span>

| <span data-ttu-id="499be-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="499be-109">Property name</span></span>                   | <span data-ttu-id="499be-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="499be-110">Type</span></span>    | <span data-ttu-id="499be-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="499be-111">Description</span></span>
|:--------------------------------|:--------|:---------------------------------
| <span data-ttu-id="499be-112">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="499be-112">**allowMultipleLines**</span></span>          | <span data-ttu-id="499be-113">booliano</span><span class="sxs-lookup"><span data-stu-id="499be-113">boolean</span></span> | <span data-ttu-id="499be-114">Se deseja permitir várias linhas de texto.</span><span class="sxs-lookup"><span data-stu-id="499be-114">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="499be-115">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="499be-115">**appendChangesToExistingText**</span></span> | <span data-ttu-id="499be-116">booliano</span><span class="sxs-lookup"><span data-stu-id="499be-116">boolean</span></span> | <span data-ttu-id="499be-117">Se as atualizações nesta coluna devem substituir o texto existente ou acrescentar a ele.</span><span class="sxs-lookup"><span data-stu-id="499be-117">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="499be-118">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="499be-118">**linesForEditing**</span></span>             | <span data-ttu-id="499be-119">int32</span><span class="sxs-lookup"><span data-stu-id="499be-119">int32</span></span>   | <span data-ttu-id="499be-120">O tamanho da caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="499be-120">The size of the text box.</span></span>
| <span data-ttu-id="499be-121">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="499be-121">**maxLength**</span></span>                   | <span data-ttu-id="499be-122">int32</span><span class="sxs-lookup"><span data-stu-id="499be-122">int32</span></span>   | <span data-ttu-id="499be-123">O número máximo de caracteres para o valor.</span><span class="sxs-lookup"><span data-stu-id="499be-123">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="499be-124">**textType**</span><span class="sxs-lookup"><span data-stu-id="499be-124">**textType**</span></span>                    | <span data-ttu-id="499be-125">string</span><span class="sxs-lookup"><span data-stu-id="499be-125">string</span></span>  | <span data-ttu-id="499be-126">O tipo de texto sendo armazenado.</span><span class="sxs-lookup"><span data-stu-id="499be-126">The type of text being stored.</span></span> <span data-ttu-id="499be-127">Deve ser `plain` ou `richText`</span><span class="sxs-lookup"><span data-stu-id="499be-127">Must be one of `plain` or `richText`</span></span>

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

