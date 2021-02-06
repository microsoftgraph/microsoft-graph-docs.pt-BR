---
title: Tipo de recurso userAttributeValuesItem
description: Usado para preencher os valores de um atributo de fluxo de usuário dentro de um fluxo de usuário quando há várias seleções para escolher.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 64b2416cd6fd0e8c92d9a00ff2d599226e3cd02c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133018"
---
# <a name="userattributevaluesitem-resource-type"></a><span data-ttu-id="0afcc-103">Tipo de recurso userAttributeValuesItem</span><span class="sxs-lookup"><span data-stu-id="0afcc-103">userAttributeValuesItem resource type</span></span>

<span data-ttu-id="0afcc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0afcc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0afcc-105">Usado para preencher os valores de um atributo de fluxo de usuário dentro de um fluxo de usuário quando há várias seleções para escolher.</span><span class="sxs-lookup"><span data-stu-id="0afcc-105">Used to populate the values for a user flow attribute within a user flow when there are multiple selections to choose from.</span></span> <span data-ttu-id="0afcc-106">userAttributeValuesItem é aplicável ao userInputTypes , e para `radioSingleSelect` `dropdownSingleSelect` uma `checkboxMultiSelect` [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md).</span><span class="sxs-lookup"><span data-stu-id="0afcc-106">userAttributeValuesItem is applicable to the userInputTypes `radioSingleSelect`, `dropdownSingleSelect`, and `checkboxMultiSelect` for an [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0afcc-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0afcc-107">Properties</span></span>

|<span data-ttu-id="0afcc-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0afcc-108">Property</span></span>|<span data-ttu-id="0afcc-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0afcc-109">Type</span></span>|<span data-ttu-id="0afcc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0afcc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0afcc-111">isDefault</span><span class="sxs-lookup"><span data-stu-id="0afcc-111">isDefault</span></span>|<span data-ttu-id="0afcc-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="0afcc-112">Boolean</span></span>|<span data-ttu-id="0afcc-113">Usado para definir o valor como padrão.</span><span class="sxs-lookup"><span data-stu-id="0afcc-113">Used to set the value as the default.</span></span>|
|<span data-ttu-id="0afcc-114">nome</span><span class="sxs-lookup"><span data-stu-id="0afcc-114">name</span></span>|<span data-ttu-id="0afcc-115">String</span><span class="sxs-lookup"><span data-stu-id="0afcc-115">String</span></span>|<span data-ttu-id="0afcc-116">O nome de exibição da propriedade exibida para o usuário final no fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="0afcc-116">The display name of the property displayed to the end user in the user flow.</span></span>|
|<span data-ttu-id="0afcc-117">value</span><span class="sxs-lookup"><span data-stu-id="0afcc-117">value</span></span>|<span data-ttu-id="0afcc-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0afcc-118">String</span></span>|<span data-ttu-id="0afcc-119">O valor que é definido quando esse item é selecionado.</span><span class="sxs-lookup"><span data-stu-id="0afcc-119">The value that is set when this item is selected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0afcc-120">Relações</span><span class="sxs-lookup"><span data-stu-id="0afcc-120">Relationships</span></span>

<span data-ttu-id="0afcc-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0afcc-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0afcc-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0afcc-122">JSON representation</span></span>

<span data-ttu-id="0afcc-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0afcc-123">The following is a JSON representation of the resource.</span></span>
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
