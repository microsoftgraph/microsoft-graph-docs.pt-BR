---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ChoiceColumn
localization_priority: Normal
ms.openlocfilehash: 21405fe3aa28e0eef1233cd6f27e63568fb4b00e
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482214"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="a73b5-102">Tipo de recurso ChoiceColumn</span><span class="sxs-lookup"><span data-stu-id="a73b5-102">ChoiceColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a73b5-103">O **choiceColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna podem ser selecionados em uma lista de opções.</span><span class="sxs-lookup"><span data-stu-id="a73b5-103">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a73b5-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a73b5-104">JSON representation</span></span>

<span data-ttu-id="a73b5-105">Aqui está uma representação JSON de um recurso **choiceColumn**.</span><span class="sxs-lookup"><span data-stu-id="a73b5-105">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="a73b5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a73b5-106">Properties</span></span>

| <span data-ttu-id="a73b5-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="a73b5-107">Property name</span></span>      | <span data-ttu-id="a73b5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a73b5-108">Type</span></span>               | <span data-ttu-id="a73b5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a73b5-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="a73b5-110">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="a73b5-110">**allowTextEntry**</span></span> | <span data-ttu-id="a73b5-111">booliano</span><span class="sxs-lookup"><span data-stu-id="a73b5-111">boolean</span></span>            | <span data-ttu-id="a73b5-112">Se verdadeiro, permite valores personalizados que não estão em opções configuradas.</span><span class="sxs-lookup"><span data-stu-id="a73b5-112">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="a73b5-113">**choices**</span><span class="sxs-lookup"><span data-stu-id="a73b5-113">**choices**</span></span>        | <span data-ttu-id="a73b5-114">collection(string)</span><span class="sxs-lookup"><span data-stu-id="a73b5-114">collection(string)</span></span> | <span data-ttu-id="a73b5-115">A lista de valores disponíveis para essa coluna.</span><span class="sxs-lookup"><span data-stu-id="a73b5-115">The list of values available for this column.</span></span>
| <span data-ttu-id="a73b5-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="a73b5-116">**displayAs**</span></span>      | <span data-ttu-id="a73b5-117">string</span><span class="sxs-lookup"><span data-stu-id="a73b5-117">string</span></span>             | <span data-ttu-id="a73b5-118">Como as opções devem ser apresentadas na UX.</span><span class="sxs-lookup"><span data-stu-id="a73b5-118">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="a73b5-119">Deve ser `checkBoxes`, `dropDownMenu` ou `radioButtons`</span><span class="sxs-lookup"><span data-stu-id="a73b5-119">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/choicecolumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
