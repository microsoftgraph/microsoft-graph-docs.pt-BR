---
author: JeremyKelley
description: O choiceColumn em um recurso columnDefinition indica que os valores da coluna podem ser selecionados em uma lista de opções.
ms.date: 09/11/2017
title: ChoiceColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 72ef8adb96614fc32b9aee8141eb19248e963639
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973482"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="10111-103">Tipo de recurso ChoiceColumn</span><span class="sxs-lookup"><span data-stu-id="10111-103">ChoiceColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10111-104">O **choiceColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna podem ser selecionados em uma lista de opções.</span><span class="sxs-lookup"><span data-stu-id="10111-104">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="10111-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10111-105">JSON representation</span></span>

<span data-ttu-id="10111-106">Aqui está uma representação JSON de um recurso **choiceColumn**.</span><span class="sxs-lookup"><span data-stu-id="10111-106">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="10111-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10111-107">Properties</span></span>

| <span data-ttu-id="10111-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="10111-108">Property name</span></span>      | <span data-ttu-id="10111-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="10111-109">Type</span></span>               | <span data-ttu-id="10111-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="10111-110">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="10111-111">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="10111-111">**allowTextEntry**</span></span> | <span data-ttu-id="10111-112">booliano</span><span class="sxs-lookup"><span data-stu-id="10111-112">boolean</span></span>            | <span data-ttu-id="10111-113">Se verdadeiro, permite valores personalizados que não estão em opções configuradas.</span><span class="sxs-lookup"><span data-stu-id="10111-113">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="10111-114">**choices**</span><span class="sxs-lookup"><span data-stu-id="10111-114">**choices**</span></span>        | <span data-ttu-id="10111-115">collection(string)</span><span class="sxs-lookup"><span data-stu-id="10111-115">collection(string)</span></span> | <span data-ttu-id="10111-116">A lista de valores disponíveis para essa coluna.</span><span class="sxs-lookup"><span data-stu-id="10111-116">The list of values available for this column.</span></span>
| <span data-ttu-id="10111-117">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="10111-117">**displayAs**</span></span>      | <span data-ttu-id="10111-118">string</span><span class="sxs-lookup"><span data-stu-id="10111-118">string</span></span>             | <span data-ttu-id="10111-119">Como as opções devem ser apresentadas na UX.</span><span class="sxs-lookup"><span data-stu-id="10111-119">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="10111-120">Deve ser `checkBoxes`, `dropDownMenu` ou `radioButtons`</span><span class="sxs-lookup"><span data-stu-id="10111-120">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn",
  "suppressions": []
}
-->
