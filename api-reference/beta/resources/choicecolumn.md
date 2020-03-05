---
author: JeremyKelley
description: O choiceColumn em um recurso columnDefinition indica que os valores da coluna podem ser selecionados em uma lista de opções.
ms.date: 09/11/2017
title: ChoiceColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8b9b6db64bb1215a4be3fde10bce1a40bb5ffce3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507681"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="23e02-103">Tipo de recurso ChoiceColumn</span><span class="sxs-lookup"><span data-stu-id="23e02-103">ChoiceColumn resource type</span></span>

<span data-ttu-id="23e02-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="23e02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23e02-105">O **choiceColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna podem ser selecionados em uma lista de opções.</span><span class="sxs-lookup"><span data-stu-id="23e02-105">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="23e02-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23e02-106">JSON representation</span></span>

<span data-ttu-id="23e02-107">Aqui está uma representação JSON de um recurso **choiceColumn**.</span><span class="sxs-lookup"><span data-stu-id="23e02-107">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="23e02-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23e02-108">Properties</span></span>

| <span data-ttu-id="23e02-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="23e02-109">Property name</span></span>      | <span data-ttu-id="23e02-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="23e02-110">Type</span></span>               | <span data-ttu-id="23e02-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="23e02-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="23e02-112">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="23e02-112">**allowTextEntry**</span></span> | <span data-ttu-id="23e02-113">booliano</span><span class="sxs-lookup"><span data-stu-id="23e02-113">boolean</span></span>            | <span data-ttu-id="23e02-114">Se verdadeiro, permite valores personalizados que não estão em opções configuradas.</span><span class="sxs-lookup"><span data-stu-id="23e02-114">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="23e02-115">**choices**</span><span class="sxs-lookup"><span data-stu-id="23e02-115">**choices**</span></span>        | <span data-ttu-id="23e02-116">collection(string)</span><span class="sxs-lookup"><span data-stu-id="23e02-116">collection(string)</span></span> | <span data-ttu-id="23e02-117">A lista de valores disponíveis para essa coluna.</span><span class="sxs-lookup"><span data-stu-id="23e02-117">The list of values available for this column.</span></span>
| <span data-ttu-id="23e02-118">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="23e02-118">**displayAs**</span></span>      | <span data-ttu-id="23e02-119">string</span><span class="sxs-lookup"><span data-stu-id="23e02-119">string</span></span>             | <span data-ttu-id="23e02-120">Como as opções devem ser apresentadas na UX.</span><span class="sxs-lookup"><span data-stu-id="23e02-120">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="23e02-121">Deve ser `checkBoxes`, `dropDownMenu` ou `radioButtons`</span><span class="sxs-lookup"><span data-stu-id="23e02-121">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


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
