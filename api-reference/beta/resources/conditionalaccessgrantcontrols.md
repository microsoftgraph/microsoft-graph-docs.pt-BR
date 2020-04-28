---
title: tipo de recurso conditionalAccessGrantControls
description: Representa os controles de concessão que devem ser atendidos para passar a política.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a4312accf3b908689a0037d3c16a7ba2242c2ddf
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916779"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="4bbb2-103">tipo de recurso conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="4bbb2-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="4bbb2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4bbb2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bbb2-105">Representa os controles de concessão que devem ser atendidos para passar a política.</span><span class="sxs-lookup"><span data-stu-id="4bbb2-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="4bbb2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4bbb2-106">Properties</span></span>

| <span data-ttu-id="4bbb2-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4bbb2-107">Property</span></span> | <span data-ttu-id="4bbb2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="4bbb2-108">Type</span></span> | <span data-ttu-id="4bbb2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bbb2-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="4bbb2-110">operator</span><span class="sxs-lookup"><span data-stu-id="4bbb2-110">operator</span></span> | <span data-ttu-id="4bbb2-111">String</span><span class="sxs-lookup"><span data-stu-id="4bbb2-111">String</span></span> | <span data-ttu-id="4bbb2-112">Define o relacionamento dos controles de concessão.</span><span class="sxs-lookup"><span data-stu-id="4bbb2-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="4bbb2-113">Valores possíveis: `AND`, `OR`.</span><span class="sxs-lookup"><span data-stu-id="4bbb2-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="4bbb2-114">builtInControls</span><span class="sxs-lookup"><span data-stu-id="4bbb2-114">builtInControls</span></span> | <span data-ttu-id="4bbb2-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4bbb2-115">String collection</span></span> | <span data-ttu-id="4bbb2-116">Lista de valores de controles internos exigidos pela política.</span><span class="sxs-lookup"><span data-stu-id="4bbb2-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="4bbb2-117">Valores possíveis: `Block`, `Mfa`, `CompliantDevice` `DomainJoinedDevice`,, `ApprovedApplication`,`CompliantApplication`</span><span class="sxs-lookup"><span data-stu-id="4bbb2-117">Possible values: `Block`, `Mfa`, `CompliantDevice`, `DomainJoinedDevice`, `ApprovedApplication`, `CompliantApplication`</span></span> |
| <span data-ttu-id="4bbb2-118">customAuthenticationFactors</span><span class="sxs-lookup"><span data-stu-id="4bbb2-118">customAuthenticationFactors</span></span> | <span data-ttu-id="4bbb2-119">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4bbb2-119">String collection</span></span> | <span data-ttu-id="4bbb2-120">Lista de IDs de controles personalizados exigidos pela política.</span><span class="sxs-lookup"><span data-stu-id="4bbb2-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="4bbb2-121">Saiba mais sobre os controles personalizados aqui:https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span><span class="sxs-lookup"><span data-stu-id="4bbb2-121">Learn more about custom controls here: https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span></span> |
| <span data-ttu-id="4bbb2-122">termsOfUse</span><span class="sxs-lookup"><span data-stu-id="4bbb2-122">termsOfUse</span></span> | <span data-ttu-id="4bbb2-123">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4bbb2-123">String collection</span></span> | <span data-ttu-id="4bbb2-124">Lista de [termos de uso](agreement.md) IDs exigidos pela política.</span><span class="sxs-lookup"><span data-stu-id="4bbb2-124">List of [terms of use](agreement.md) IDs required by the policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4bbb2-125">Relações</span><span class="sxs-lookup"><span data-stu-id="4bbb2-125">Relationships</span></span>

<span data-ttu-id="4bbb2-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4bbb2-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4bbb2-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4bbb2-127">JSON representation</span></span>

<span data-ttu-id="4bbb2-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4bbb2-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "operator",
    "builtInControls",
    "customAuthenticationFactors",
    "termsOfUse"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessGrantControls",
  "baseType": null
}-->

```json
{
  "builtInControls": ["String"],
  "customAuthenticationFactors": ["String"],
  "operator": "String",
  "termsOfUse": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessGrantControls resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->