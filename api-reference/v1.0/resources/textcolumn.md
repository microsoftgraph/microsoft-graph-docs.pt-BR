---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: 1e10997bd70f97fa91177aee48a6ffcecff40ab5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456994"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="70e4e-102">Tipo de recurso TextColumn</span><span class="sxs-lookup"><span data-stu-id="70e4e-102">TextColumn resource type</span></span>

<span data-ttu-id="70e4e-103">**textColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são texto.</span><span class="sxs-lookup"><span data-stu-id="70e4e-103">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="70e4e-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="70e4e-104">JSON representation</span></span>

<span data-ttu-id="70e4e-105">Aqui está uma representação JSON de um recurso **textColumn**.</span><span class="sxs-lookup"><span data-stu-id="70e4e-105">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="70e4e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="70e4e-106">Properties</span></span>

| <span data-ttu-id="70e4e-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="70e4e-107">Property name</span></span>                   | <span data-ttu-id="70e4e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="70e4e-108">Type</span></span>    | <span data-ttu-id="70e4e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="70e4e-109">Description</span></span>
|:--------------------------------|:--------|:---------------------------------
| <span data-ttu-id="70e4e-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="70e4e-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="70e4e-111">booliano</span><span class="sxs-lookup"><span data-stu-id="70e4e-111">boolean</span></span> | <span data-ttu-id="70e4e-112">Se deseja permitir várias linhas de texto.</span><span class="sxs-lookup"><span data-stu-id="70e4e-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="70e4e-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="70e4e-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="70e4e-114">booliano</span><span class="sxs-lookup"><span data-stu-id="70e4e-114">boolean</span></span> | <span data-ttu-id="70e4e-115">Se as atualizações nesta coluna devem substituir o texto existente ou acrescentar a ele.</span><span class="sxs-lookup"><span data-stu-id="70e4e-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="70e4e-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="70e4e-116">**linesForEditing**</span></span>             | <span data-ttu-id="70e4e-117">Int32</span><span class="sxs-lookup"><span data-stu-id="70e4e-117">int32</span></span>   | <span data-ttu-id="70e4e-118">O tamanho da caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="70e4e-118">The size of the text box.</span></span>
| <span data-ttu-id="70e4e-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="70e4e-119">**maxLength**</span></span>                   | <span data-ttu-id="70e4e-120">Int32</span><span class="sxs-lookup"><span data-stu-id="70e4e-120">int32</span></span>   | <span data-ttu-id="70e4e-121">O número máximo de caracteres para o valor.</span><span class="sxs-lookup"><span data-stu-id="70e4e-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="70e4e-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="70e4e-122">**textType**</span></span>                    | <span data-ttu-id="70e4e-123">string</span><span class="sxs-lookup"><span data-stu-id="70e4e-123">string</span></span>  | <span data-ttu-id="70e4e-124">O tipo de texto sendo armazenado.</span><span class="sxs-lookup"><span data-stu-id="70e4e-124">The type of text being stored.</span></span> <span data-ttu-id="70e4e-125">Deve ser `plain` ou `richText`</span><span class="sxs-lookup"><span data-stu-id="70e4e-125">Must be one of `plain` or `richText`</span></span>

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
