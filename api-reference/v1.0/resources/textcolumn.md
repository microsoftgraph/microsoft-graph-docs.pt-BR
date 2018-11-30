---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
ms.openlocfilehash: 810554620e747d3160a6d8c74913518b8590c19d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006704"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="f26e7-102">Tipo de recurso TextColumn</span><span class="sxs-lookup"><span data-stu-id="f26e7-102">TextColumn resource type</span></span>

<span data-ttu-id="f26e7-103">**textColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são texto.</span><span class="sxs-lookup"><span data-stu-id="f26e7-103">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f26e7-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f26e7-104">JSON representation</span></span>

<span data-ttu-id="f26e7-105">Aqui está uma representação JSON de um recurso **textColumn**.</span><span class="sxs-lookup"><span data-stu-id="f26e7-105">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="f26e7-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f26e7-106">Properties</span></span>

| <span data-ttu-id="f26e7-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="f26e7-107">Property name</span></span>                   | <span data-ttu-id="f26e7-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f26e7-108">Type</span></span>    | <span data-ttu-id="f26e7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f26e7-109">Description</span></span>
|:--------------------------------|:--------|:---------------------------------
| <span data-ttu-id="f26e7-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="f26e7-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="f26e7-111">booliano</span><span class="sxs-lookup"><span data-stu-id="f26e7-111">boolean</span></span> | <span data-ttu-id="f26e7-112">Se deseja permitir várias linhas de texto.</span><span class="sxs-lookup"><span data-stu-id="f26e7-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="f26e7-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="f26e7-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="f26e7-114">booliano</span><span class="sxs-lookup"><span data-stu-id="f26e7-114">boolean</span></span> | <span data-ttu-id="f26e7-115">Se as atualizações nesta coluna devem substituir o texto existente ou acrescentar a ele.</span><span class="sxs-lookup"><span data-stu-id="f26e7-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="f26e7-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="f26e7-116">**linesForEditing**</span></span>             | <span data-ttu-id="f26e7-117">int32</span><span class="sxs-lookup"><span data-stu-id="f26e7-117">int32</span></span>   | <span data-ttu-id="f26e7-118">O tamanho da caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="f26e7-118">The size of the text box.</span></span>
| <span data-ttu-id="f26e7-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="f26e7-119">**maxLength**</span></span>                   | <span data-ttu-id="f26e7-120">int32</span><span class="sxs-lookup"><span data-stu-id="f26e7-120">int32</span></span>   | <span data-ttu-id="f26e7-121">O número máximo de caracteres para o valor.</span><span class="sxs-lookup"><span data-stu-id="f26e7-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="f26e7-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="f26e7-122">**textType**</span></span>                    | <span data-ttu-id="f26e7-123">string</span><span class="sxs-lookup"><span data-stu-id="f26e7-123">string</span></span>  | <span data-ttu-id="f26e7-124">O tipo de texto sendo armazenado.</span><span class="sxs-lookup"><span data-stu-id="f26e7-124">The type of text being stored.</span></span> <span data-ttu-id="f26e7-125">Deve ser `plain` ou `richText`</span><span class="sxs-lookup"><span data-stu-id="f26e7-125">Must be one of `plain` or `richText`</span></span>

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
