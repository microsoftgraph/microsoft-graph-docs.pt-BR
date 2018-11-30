---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ChoiceColumn
ms.openlocfilehash: 659ece2eab255fe7b55a258b0980eda4e7bde5b2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033156"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="055ce-102">Tipo de recurso ChoiceColumn</span><span class="sxs-lookup"><span data-stu-id="055ce-102">ChoiceColumn resource type</span></span>

> <span data-ttu-id="055ce-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="055ce-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="055ce-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="055ce-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="055ce-105">O **choiceColumn** em um recurso [columnDefinition](columndefinition.md) indica que os valores da coluna podem ser selecionados em uma lista de opções.</span><span class="sxs-lookup"><span data-stu-id="055ce-105">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="055ce-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="055ce-106">JSON representation</span></span>

<span data-ttu-id="055ce-107">Aqui está uma representação JSON de um recurso **choiceColumn**.</span><span class="sxs-lookup"><span data-stu-id="055ce-107">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="055ce-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="055ce-108">Properties</span></span>

| <span data-ttu-id="055ce-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="055ce-109">Property name</span></span>      | <span data-ttu-id="055ce-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="055ce-110">Type</span></span>               | <span data-ttu-id="055ce-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="055ce-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="055ce-112">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="055ce-112">**allowTextEntry**</span></span> | <span data-ttu-id="055ce-113">booliano</span><span class="sxs-lookup"><span data-stu-id="055ce-113">boolean</span></span>            | <span data-ttu-id="055ce-114">Se verdadeiro, permite valores personalizados que não estão em opções configuradas.</span><span class="sxs-lookup"><span data-stu-id="055ce-114">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="055ce-115">**choices**</span><span class="sxs-lookup"><span data-stu-id="055ce-115">**choices**</span></span>        | <span data-ttu-id="055ce-116">collection(string)</span><span class="sxs-lookup"><span data-stu-id="055ce-116">collection(string)</span></span> | <span data-ttu-id="055ce-117">A lista de valores disponíveis para essa coluna.</span><span class="sxs-lookup"><span data-stu-id="055ce-117">The list of values available for this column.</span></span>
| <span data-ttu-id="055ce-118">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="055ce-118">**displayAs**</span></span>      | <span data-ttu-id="055ce-119">string</span><span class="sxs-lookup"><span data-stu-id="055ce-119">string</span></span>             | <span data-ttu-id="055ce-120">Como as opções devem ser apresentadas na UX.</span><span class="sxs-lookup"><span data-stu-id="055ce-120">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="055ce-121">Deve ser `checkBoxes`, `dropDownMenu` ou `radioButtons`</span><span class="sxs-lookup"><span data-stu-id="055ce-121">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn"
} -->
