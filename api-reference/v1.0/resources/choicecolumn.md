---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ChoiceColumn
ms.openlocfilehash: 6841f453cdfd423ead3edeea5895242a28b998f3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004053"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="9dff2-102">Tipo de recurso ChoiceColumn</span><span class="sxs-lookup"><span data-stu-id="9dff2-102">ChoiceColumn resource type</span></span>

<span data-ttu-id="9dff2-103">O **choiceColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna podem ser selecionados em uma lista de opções.</span><span class="sxs-lookup"><span data-stu-id="9dff2-103">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9dff2-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9dff2-104">JSON representation</span></span>

<span data-ttu-id="9dff2-105">Aqui está uma representação JSON de um recurso **choiceColumn**.</span><span class="sxs-lookup"><span data-stu-id="9dff2-105">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="9dff2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9dff2-106">Properties</span></span>

| <span data-ttu-id="9dff2-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="9dff2-107">Property name</span></span>      | <span data-ttu-id="9dff2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9dff2-108">Type</span></span>               | <span data-ttu-id="9dff2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9dff2-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="9dff2-110">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="9dff2-110">**allowTextEntry**</span></span> | <span data-ttu-id="9dff2-111">booliano</span><span class="sxs-lookup"><span data-stu-id="9dff2-111">boolean</span></span>            | <span data-ttu-id="9dff2-112">Se verdadeiro, permite valores personalizados que não estão em opções configuradas.</span><span class="sxs-lookup"><span data-stu-id="9dff2-112">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="9dff2-113">**choices**</span><span class="sxs-lookup"><span data-stu-id="9dff2-113">**choices**</span></span>        | <span data-ttu-id="9dff2-114">collection(string)</span><span class="sxs-lookup"><span data-stu-id="9dff2-114">collection(string)</span></span> | <span data-ttu-id="9dff2-115">A lista de valores disponíveis para essa coluna.</span><span class="sxs-lookup"><span data-stu-id="9dff2-115">The list of values available for this column.</span></span>
| <span data-ttu-id="9dff2-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="9dff2-116">**displayAs**</span></span>      | <span data-ttu-id="9dff2-117">string</span><span class="sxs-lookup"><span data-stu-id="9dff2-117">string</span></span>             | <span data-ttu-id="9dff2-118">Como as opções devem ser apresentadas na UX.</span><span class="sxs-lookup"><span data-stu-id="9dff2-118">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="9dff2-119">Deve ser `checkBoxes`, `dropDownMenu` ou `radioButtons`</span><span class="sxs-lookup"><span data-stu-id="9dff2-119">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


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
