---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: TextColumn
ms.openlocfilehash: 80e41b379b9b4ce51a3ee6c910447a22f43356c3
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="c1fa1-102">Tipo de recurso TextColumn</span><span class="sxs-lookup"><span data-stu-id="c1fa1-102">TextColumn resource type</span></span>

<span data-ttu-id="c1fa1-103">**textColumn** em um recurso [columnDefinition](columnDefinition.md) indica que os valores da coluna são texto.</span><span class="sxs-lookup"><span data-stu-id="c1fa1-103">The **textColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1fa1-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c1fa1-104">JSON representation</span></span>

<span data-ttu-id="c1fa1-105">Aqui está uma representação JSON de um recurso **textColumn**.</span><span class="sxs-lookup"><span data-stu-id="c1fa1-105">Here is a JSON representation of a **baseItem** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="c1fa1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c1fa1-106">Properties</span></span>

| <span data-ttu-id="c1fa1-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="c1fa1-107">Property name</span></span>                   | <span data-ttu-id="c1fa1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1fa1-108">Type</span></span>   | <span data-ttu-id="c1fa1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1fa1-109">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="c1fa1-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="c1fa1-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="c1fa1-111">string</span><span class="sxs-lookup"><span data-stu-id="c1fa1-111">string</span></span> | <span data-ttu-id="c1fa1-112">Se deseja permitir várias linhas de texto.</span><span class="sxs-lookup"><span data-stu-id="c1fa1-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="c1fa1-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="c1fa1-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="c1fa1-114">string</span><span class="sxs-lookup"><span data-stu-id="c1fa1-114">string</span></span> | <span data-ttu-id="c1fa1-115">Se as atualizações nesta coluna devem substituir o texto existente ou acrescentar a ele.</span><span class="sxs-lookup"><span data-stu-id="c1fa1-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="c1fa1-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="c1fa1-116">**linesForEditing**</span></span>             | <span data-ttu-id="c1fa1-117">int</span><span class="sxs-lookup"><span data-stu-id="c1fa1-117">int</span></span>    | <span data-ttu-id="c1fa1-118">O tamanho da caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="c1fa1-118">The size of the text box.</span></span>
| <span data-ttu-id="c1fa1-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="c1fa1-119">**maxLength**</span></span>                   | <span data-ttu-id="c1fa1-120">int</span><span class="sxs-lookup"><span data-stu-id="c1fa1-120">int</span></span>    | <span data-ttu-id="c1fa1-121">O número máximo de caracteres para o valor.</span><span class="sxs-lookup"><span data-stu-id="c1fa1-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="c1fa1-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="c1fa1-122">**textType**</span></span>                    | <span data-ttu-id="c1fa1-123">string</span><span class="sxs-lookup"><span data-stu-id="c1fa1-123">string</span></span> | <span data-ttu-id="c1fa1-124">O tipo de texto sendo armazenado.</span><span class="sxs-lookup"><span data-stu-id="c1fa1-124">The type of text being stored.</span></span> <span data-ttu-id="c1fa1-125">Deve ser `plain` ou `richText`</span><span class="sxs-lookup"><span data-stu-id="c1fa1-125">Must be one of `plain` or `richText`</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn"
} -->
