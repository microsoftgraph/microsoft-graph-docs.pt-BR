---
title: tipo de recurso userAttributeValuesItem
description: Usado para preencher os valores de um atributo de fluxo de usuário dentro de um fluxo de usuário quando há várias seleções para escolher.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6fd0d582ef4dcdd83dba6947536c5acdbc14a8cb
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581286"
---
# <a name="userattributevaluesitem-resource-type"></a><span data-ttu-id="2ece9-103">tipo de recurso userAttributeValuesItem</span><span class="sxs-lookup"><span data-stu-id="2ece9-103">userAttributeValuesItem resource type</span></span>

<span data-ttu-id="2ece9-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2ece9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2ece9-105">Usado para preencher os valores de um atributo de fluxo de usuário dentro de um fluxo de usuário quando há várias seleções para escolher.</span><span class="sxs-lookup"><span data-stu-id="2ece9-105">Used to populate the values for a user flow attribute within a user flow when there are multiple selections to choose from.</span></span> <span data-ttu-id="2ece9-106">userAttributeValuesItem é aplicável ao userInputTypes `radioSingleSelect` , `dropdownSingleSelect` e `checkboxMultiSelect` para um [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md).</span><span class="sxs-lookup"><span data-stu-id="2ece9-106">userAttributeValuesItem is applicable to the userInputTypes `radioSingleSelect`, `dropdownSingleSelect`, and `checkboxMultiSelect` for an [identityUserFlowAttributeAssignment](..\resources\identityuserflowattributeassignment.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2ece9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ece9-107">Properties</span></span>

|<span data-ttu-id="2ece9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ece9-108">Property</span></span>|<span data-ttu-id="2ece9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ece9-109">Type</span></span>|<span data-ttu-id="2ece9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ece9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ece9-111">isDefault</span><span class="sxs-lookup"><span data-stu-id="2ece9-111">isDefault</span></span>|<span data-ttu-id="2ece9-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="2ece9-112">Boolean</span></span>|<span data-ttu-id="2ece9-113">Usado para definir o valor como o padrão.</span><span class="sxs-lookup"><span data-stu-id="2ece9-113">Used to set the value as the default.</span></span>|
|<span data-ttu-id="2ece9-114">nome</span><span class="sxs-lookup"><span data-stu-id="2ece9-114">name</span></span>|<span data-ttu-id="2ece9-115">String</span><span class="sxs-lookup"><span data-stu-id="2ece9-115">String</span></span>|<span data-ttu-id="2ece9-116">O nome de exibição da propriedade exibida para o usuário final no fluxo do usuário.</span><span class="sxs-lookup"><span data-stu-id="2ece9-116">The display name of the property displayed to the end user in the user flow.</span></span>|
|<span data-ttu-id="2ece9-117">value</span><span class="sxs-lookup"><span data-stu-id="2ece9-117">value</span></span>|<span data-ttu-id="2ece9-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ece9-118">String</span></span>|<span data-ttu-id="2ece9-119">O valor definido quando este item é selecionado.</span><span class="sxs-lookup"><span data-stu-id="2ece9-119">The value that is set when this item is selected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ece9-120">Relações</span><span class="sxs-lookup"><span data-stu-id="2ece9-120">Relationships</span></span>

<span data-ttu-id="2ece9-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2ece9-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ece9-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ece9-122">JSON representation</span></span>

<span data-ttu-id="2ece9-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ece9-123">The following is a JSON representation of the resource.</span></span>
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
