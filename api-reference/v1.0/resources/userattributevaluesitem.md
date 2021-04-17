---
title: Tipo de recurso userAttributeValuesItem
description: Representa valores de atributo de fluxo do usuário dentro de um fluxo de usuário.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 367f5d835f3790c589a8d7d28b7994484fd9613c
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882382"
---
# <a name="userattributevaluesitem-resource-type"></a><span data-ttu-id="fccf8-103">Tipo de recurso userAttributeValuesItem</span><span class="sxs-lookup"><span data-stu-id="fccf8-103">userAttributeValuesItem resource type</span></span>

<span data-ttu-id="fccf8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fccf8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fccf8-105">Representa valores de atributo de fluxo do usuário em um fluxo de usuário quando há várias seleções para escolher.</span><span class="sxs-lookup"><span data-stu-id="fccf8-105">Represents user flow attribute values within a user flow when there are multiple selections to choose from.</span></span>  <span data-ttu-id="fccf8-106">O userAttributeValuesItem é aplicável ao userInputTypes de , e a `radioSingleSelect` `dropdownSingleSelect` uma `checkboxMultiSelect` [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md).</span><span class="sxs-lookup"><span data-stu-id="fccf8-106">The userAttributeValuesItem is applicable to the userInputTypes of `radioSingleSelect`, `dropdownSingleSelect`, and `checkboxMultiSelect` for an [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fccf8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fccf8-107">Properties</span></span>

|<span data-ttu-id="fccf8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fccf8-108">Property</span></span>|<span data-ttu-id="fccf8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fccf8-109">Type</span></span>|<span data-ttu-id="fccf8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fccf8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fccf8-111">isDefault</span><span class="sxs-lookup"><span data-stu-id="fccf8-111">isDefault</span></span>|<span data-ttu-id="fccf8-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="fccf8-112">Boolean</span></span>|<span data-ttu-id="fccf8-113">Determina se o valor é definido como padrão.</span><span class="sxs-lookup"><span data-stu-id="fccf8-113">Determines whether the value is set as the default.</span></span>|
|<span data-ttu-id="fccf8-114">nome</span><span class="sxs-lookup"><span data-stu-id="fccf8-114">name</span></span>|<span data-ttu-id="fccf8-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fccf8-115">String</span></span>|<span data-ttu-id="fccf8-116">O nome de exibição da propriedade exibida para o usuário no fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="fccf8-116">The display name of the property displayed to the user in the user flow.</span></span>|
|<span data-ttu-id="fccf8-117">value</span><span class="sxs-lookup"><span data-stu-id="fccf8-117">value</span></span>|<span data-ttu-id="fccf8-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="fccf8-118">String</span></span>|<span data-ttu-id="fccf8-119">O valor que é definido quando esse item é selecionado.</span><span class="sxs-lookup"><span data-stu-id="fccf8-119">The value that is set when this item is selected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fccf8-120">Relações</span><span class="sxs-lookup"><span data-stu-id="fccf8-120">Relationships</span></span>

<span data-ttu-id="fccf8-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fccf8-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fccf8-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fccf8-122">JSON representation</span></span>

<span data-ttu-id="fccf8-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fccf8-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userAttributeValuesItem"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userAttributeValuesItem",
  "name": "String",
  "value": "String",
  "isDefault": "Boolean"
}
```
