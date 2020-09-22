---
author: JeremyKelley
description: O choiceColumn em um recurso columnDefinition indica que os valores da coluna podem ser selecionados em uma lista de opções.
ms.date: 09/11/2017
title: ChoiceColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: a5e6efa944756077eb29467be6e75013d4bf28aa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021984"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="bad51-103">Tipo de recurso ChoiceColumn</span><span class="sxs-lookup"><span data-stu-id="bad51-103">ChoiceColumn resource type</span></span>

<span data-ttu-id="bad51-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bad51-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bad51-105">O **choiceColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna podem ser selecionados em uma lista de opções.</span><span class="sxs-lookup"><span data-stu-id="bad51-105">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bad51-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bad51-106">JSON representation</span></span>

<span data-ttu-id="bad51-107">Aqui está uma representação JSON de um recurso **choiceColumn**.</span><span class="sxs-lookup"><span data-stu-id="bad51-107">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="bad51-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bad51-108">Properties</span></span>

| <span data-ttu-id="bad51-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="bad51-109">Property name</span></span>      | <span data-ttu-id="bad51-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bad51-110">Type</span></span>               | <span data-ttu-id="bad51-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bad51-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="bad51-112">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="bad51-112">**allowTextEntry**</span></span> | <span data-ttu-id="bad51-113">booliano</span><span class="sxs-lookup"><span data-stu-id="bad51-113">boolean</span></span>            | <span data-ttu-id="bad51-114">Se verdadeiro, permite valores personalizados que não estão em opções configuradas.</span><span class="sxs-lookup"><span data-stu-id="bad51-114">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="bad51-115">**choices**</span><span class="sxs-lookup"><span data-stu-id="bad51-115">**choices**</span></span>        | <span data-ttu-id="bad51-116">collection(string)</span><span class="sxs-lookup"><span data-stu-id="bad51-116">collection(string)</span></span> | <span data-ttu-id="bad51-117">A lista de valores disponíveis para essa coluna.</span><span class="sxs-lookup"><span data-stu-id="bad51-117">The list of values available for this column.</span></span>
| <span data-ttu-id="bad51-118">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="bad51-118">**displayAs**</span></span>      | <span data-ttu-id="bad51-119">string</span><span class="sxs-lookup"><span data-stu-id="bad51-119">string</span></span>             | <span data-ttu-id="bad51-120">Como as opções devem ser apresentadas na UX.</span><span class="sxs-lookup"><span data-stu-id="bad51-120">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="bad51-121">Deve ser `checkBoxes`, `dropDownMenu` ou `radioButtons`</span><span class="sxs-lookup"><span data-stu-id="bad51-121">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


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


