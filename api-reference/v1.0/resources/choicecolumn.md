---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ChoiceColumn
ms.openlocfilehash: c266550e8918603c3ee6104818c0aa721f1281d9
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="04f25-102">Tipo de recurso ChoiceColumn</span><span class="sxs-lookup"><span data-stu-id="04f25-102">ChoiceColumn resource type</span></span>

<span data-ttu-id="04f25-103">O **choiceColumn** em um recurso [columnDefinition](columnDefinition.md) indica que os valores da coluna podem ser selecionados em uma lista de opções.</span><span class="sxs-lookup"><span data-stu-id="04f25-103">The **choiceColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="04f25-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04f25-104">JSON representation</span></span>

<span data-ttu-id="04f25-105">Aqui está uma representação JSON de um recurso **choiceColumn**.</span><span class="sxs-lookup"><span data-stu-id="04f25-105">Here is a JSON representation of a **driveItem** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="04f25-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04f25-106">Properties</span></span>

| <span data-ttu-id="04f25-107">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="04f25-107">Property name</span></span>      | <span data-ttu-id="04f25-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="04f25-108">Type</span></span>               | <span data-ttu-id="04f25-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="04f25-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="04f25-110">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="04f25-110">**allowTextEntry**</span></span> | <span data-ttu-id="04f25-111">booliano</span><span class="sxs-lookup"><span data-stu-id="04f25-111">boolean</span></span>            | <span data-ttu-id="04f25-112">Se verdadeiro, permite valores personalizados que não estão em opções configuradas.</span><span class="sxs-lookup"><span data-stu-id="04f25-112">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="04f25-113">**choices**</span><span class="sxs-lookup"><span data-stu-id="04f25-113">**Choices**</span></span>        | <span data-ttu-id="04f25-114">collection(string)</span><span class="sxs-lookup"><span data-stu-id="04f25-114">Collection(String)</span></span> | <span data-ttu-id="04f25-115">A lista de valores disponíveis para essa coluna.</span><span class="sxs-lookup"><span data-stu-id="04f25-115">The list of values available for this column.</span></span>
| <span data-ttu-id="04f25-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="04f25-116">**displayAs**</span></span>      | <span data-ttu-id="04f25-117">string</span><span class="sxs-lookup"><span data-stu-id="04f25-117">string</span></span>             | <span data-ttu-id="04f25-118">Como as opções devem ser apresentadas na UX.</span><span class="sxs-lookup"><span data-stu-id="04f25-118">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="04f25-119">Deve ser `checkBoxes`, `dropDownMenu` ou `radioButtons`</span><span class="sxs-lookup"><span data-stu-id="04f25-119">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn"
} -->
