---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ChoiceColumn
localization_priority: Normal
ms.openlocfilehash: 3640e68902485215dda575cc93407f019007ee18
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826576"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="a0c6b-102">Tipo de recurso ChoiceColumn</span><span class="sxs-lookup"><span data-stu-id="a0c6b-102">ChoiceColumn resource type</span></span>

<span data-ttu-id="a0c6b-103">O **choiceColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna podem ser selecionados em uma lista de opções.</span><span class="sxs-lookup"><span data-stu-id="a0c6b-103">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0c6b-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0c6b-104">JSON representation</span></span>

<span data-ttu-id="a0c6b-105">Aqui está uma representação JSON de um recurso **choiceColumn**.</span><span class="sxs-lookup"><span data-stu-id="a0c6b-105">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="a0c6b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0c6b-106">Properties</span></span>

| <span data-ttu-id="a0c6b-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="a0c6b-107">Property name</span></span>      | <span data-ttu-id="a0c6b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0c6b-108">Type</span></span>               | <span data-ttu-id="a0c6b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0c6b-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="a0c6b-110">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="a0c6b-110">**allowTextEntry**</span></span> | <span data-ttu-id="a0c6b-111">booliano</span><span class="sxs-lookup"><span data-stu-id="a0c6b-111">boolean</span></span>            | <span data-ttu-id="a0c6b-112">Se verdadeiro, permite valores personalizados que não estão em opções configuradas.</span><span class="sxs-lookup"><span data-stu-id="a0c6b-112">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="a0c6b-113">**choices**</span><span class="sxs-lookup"><span data-stu-id="a0c6b-113">**choices**</span></span>        | <span data-ttu-id="a0c6b-114">collection(string)</span><span class="sxs-lookup"><span data-stu-id="a0c6b-114">collection(string)</span></span> | <span data-ttu-id="a0c6b-115">A lista de valores disponíveis para essa coluna.</span><span class="sxs-lookup"><span data-stu-id="a0c6b-115">The list of values available for this column.</span></span>
| <span data-ttu-id="a0c6b-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="a0c6b-116">**displayAs**</span></span>      | <span data-ttu-id="a0c6b-117">string</span><span class="sxs-lookup"><span data-stu-id="a0c6b-117">string</span></span>             | <span data-ttu-id="a0c6b-118">Como as opções devem ser apresentadas na UX.</span><span class="sxs-lookup"><span data-stu-id="a0c6b-118">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="a0c6b-119">Deve ser `checkBoxes`, `dropDownMenu` ou `radioButtons`</span><span class="sxs-lookup"><span data-stu-id="a0c6b-119">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/choicecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(checkBoxes,dropDownMenu,radioButtons) are in resource, but () are in table"
  ],
  "tocPath": "Resources/ChoiceColumn"
} -->
