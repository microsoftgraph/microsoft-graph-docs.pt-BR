---
author: JeremyKelley
ms.date: 09/11/2017
title: ChoiceColumn
localization_priority: Normal
description: O choiceColumn em um recurso columnDefinition indica que os valores da coluna podem ser selecionados em uma lista de opções.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5c31dfd2630317d7c2e9110ee00262e9f332c583
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238530"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="1e8a6-103">Tipo de recurso ChoiceColumn</span><span class="sxs-lookup"><span data-stu-id="1e8a6-103">ChoiceColumn resource type</span></span>

<span data-ttu-id="1e8a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e8a6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1e8a6-105">O **choiceColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna podem ser selecionados em uma lista de opções.</span><span class="sxs-lookup"><span data-stu-id="1e8a6-105">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e8a6-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1e8a6-106">JSON representation</span></span>

<span data-ttu-id="1e8a6-107">Aqui está uma representação JSON de um recurso **choiceColumn**.</span><span class="sxs-lookup"><span data-stu-id="1e8a6-107">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="1e8a6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1e8a6-108">Properties</span></span>

| <span data-ttu-id="1e8a6-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="1e8a6-109">Property name</span></span>      | <span data-ttu-id="1e8a6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e8a6-110">Type</span></span>               | <span data-ttu-id="1e8a6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e8a6-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="1e8a6-112">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="1e8a6-112">**allowTextEntry**</span></span> | <span data-ttu-id="1e8a6-113">booliano</span><span class="sxs-lookup"><span data-stu-id="1e8a6-113">boolean</span></span>            | <span data-ttu-id="1e8a6-114">Se verdadeiro, permite valores personalizados que não estão em opções configuradas.</span><span class="sxs-lookup"><span data-stu-id="1e8a6-114">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="1e8a6-115">**choices**</span><span class="sxs-lookup"><span data-stu-id="1e8a6-115">**choices**</span></span>        | <span data-ttu-id="1e8a6-116">collection(string)</span><span class="sxs-lookup"><span data-stu-id="1e8a6-116">collection(string)</span></span> | <span data-ttu-id="1e8a6-117">A lista de valores disponíveis para essa coluna.</span><span class="sxs-lookup"><span data-stu-id="1e8a6-117">The list of values available for this column.</span></span>
| <span data-ttu-id="1e8a6-118">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="1e8a6-118">**displayAs**</span></span>      | <span data-ttu-id="1e8a6-119">string</span><span class="sxs-lookup"><span data-stu-id="1e8a6-119">string</span></span>             | <span data-ttu-id="1e8a6-120">Como as opções devem ser apresentadas na UX.</span><span class="sxs-lookup"><span data-stu-id="1e8a6-120">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="1e8a6-121">Deve ser `checkBoxes`, `dropDownMenu` ou `radioButtons`</span><span class="sxs-lookup"><span data-stu-id="1e8a6-121">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


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

