---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: TextColumn
localization_priority: Normal
ms.openlocfilehash: c69dc7c30bff0f43327ec256af6071e34de6b898
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582889"
---
# <a name="textcolumn-resource-type"></a><span data-ttu-id="7ba4b-102">Tipo de recurso TextColumn</span><span class="sxs-lookup"><span data-stu-id="7ba4b-102">TextColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ba4b-103">**textColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna são texto.</span><span class="sxs-lookup"><span data-stu-id="7ba4b-103">The **textColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values are text.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ba4b-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ba4b-104">JSON representation</span></span>

<span data-ttu-id="7ba4b-105">Aqui está uma representação JSON de um recurso **textColumn**.</span><span class="sxs-lookup"><span data-stu-id="7ba4b-105">Here is a JSON representation of a **textColumn** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="7ba4b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ba4b-106">Properties</span></span>

| <span data-ttu-id="7ba4b-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="7ba4b-107">Property name</span></span>                   | <span data-ttu-id="7ba4b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ba4b-108">Type</span></span>   | <span data-ttu-id="7ba4b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ba4b-109">Description</span></span>
|:--------------------------------|:-------|:-----------------------------------------------
| <span data-ttu-id="7ba4b-110">**allowMultipleLines**</span><span class="sxs-lookup"><span data-stu-id="7ba4b-110">**allowMultipleLines**</span></span>          | <span data-ttu-id="7ba4b-111">string</span><span class="sxs-lookup"><span data-stu-id="7ba4b-111">string</span></span> | <span data-ttu-id="7ba4b-112">Se deseja permitir várias linhas de texto.</span><span class="sxs-lookup"><span data-stu-id="7ba4b-112">Whether to allow multiple lines of text.</span></span>
| <span data-ttu-id="7ba4b-113">**appendChangesToExistingText**</span><span class="sxs-lookup"><span data-stu-id="7ba4b-113">**appendChangesToExistingText**</span></span> | <span data-ttu-id="7ba4b-114">string</span><span class="sxs-lookup"><span data-stu-id="7ba4b-114">string</span></span> | <span data-ttu-id="7ba4b-115">Se as atualizações nesta coluna devem substituir o texto existente ou acrescentar a ele.</span><span class="sxs-lookup"><span data-stu-id="7ba4b-115">Whether updates to this column should replace existing text, or append to it.</span></span>
| <span data-ttu-id="7ba4b-116">**linesForEditing**</span><span class="sxs-lookup"><span data-stu-id="7ba4b-116">**linesForEditing**</span></span>             | <span data-ttu-id="7ba4b-117">int</span><span class="sxs-lookup"><span data-stu-id="7ba4b-117">int</span></span>    | <span data-ttu-id="7ba4b-118">O tamanho da caixa de texto.</span><span class="sxs-lookup"><span data-stu-id="7ba4b-118">The size of the text box.</span></span>
| <span data-ttu-id="7ba4b-119">**maxLength**</span><span class="sxs-lookup"><span data-stu-id="7ba4b-119">**maxLength**</span></span>                   | <span data-ttu-id="7ba4b-120">int</span><span class="sxs-lookup"><span data-stu-id="7ba4b-120">int</span></span>    | <span data-ttu-id="7ba4b-121">O número máximo de caracteres para o valor.</span><span class="sxs-lookup"><span data-stu-id="7ba4b-121">The maximum number of characters for the value.</span></span>
| <span data-ttu-id="7ba4b-122">**textType**</span><span class="sxs-lookup"><span data-stu-id="7ba4b-122">**textType**</span></span>                    | <span data-ttu-id="7ba4b-123">string</span><span class="sxs-lookup"><span data-stu-id="7ba4b-123">string</span></span> | <span data-ttu-id="7ba4b-124">O tipo de texto sendo armazenado.</span><span class="sxs-lookup"><span data-stu-id="7ba4b-124">The type of text being stored.</span></span> <span data-ttu-id="7ba4b-125">Deve ser `plain` ou `richText`</span><span class="sxs-lookup"><span data-stu-id="7ba4b-125">Must be one of `plain` or `richText`</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/TextColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/textColumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
