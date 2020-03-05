---
title: tipo de recurso conditionalAccessGrantControls
description: Representa os controles de concessão que devem ser atendidos para passar a política.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b91afb44cc43c3c6ac4970afc36914abcb08c4c9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507545"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="0ec15-103">tipo de recurso conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="0ec15-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="0ec15-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0ec15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ec15-105">Representa os controles de concessão que devem ser atendidos para passar a política.</span><span class="sxs-lookup"><span data-stu-id="0ec15-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="0ec15-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ec15-106">Properties</span></span>

| <span data-ttu-id="0ec15-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ec15-107">Property</span></span> | <span data-ttu-id="0ec15-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ec15-108">Type</span></span> | <span data-ttu-id="0ec15-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ec15-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="0ec15-110">operator</span><span class="sxs-lookup"><span data-stu-id="0ec15-110">operator</span></span> | <span data-ttu-id="0ec15-111">String</span><span class="sxs-lookup"><span data-stu-id="0ec15-111">String</span></span> | <span data-ttu-id="0ec15-112">Define o relacionamento dos controles de concessão.</span><span class="sxs-lookup"><span data-stu-id="0ec15-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="0ec15-113">Valores possíveis: `AND`, `OR`.</span><span class="sxs-lookup"><span data-stu-id="0ec15-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="0ec15-114">builtInControls</span><span class="sxs-lookup"><span data-stu-id="0ec15-114">builtInControls</span></span> | <span data-ttu-id="0ec15-115">String collection</span><span class="sxs-lookup"><span data-stu-id="0ec15-115">String collection</span></span> | <span data-ttu-id="0ec15-116">Lista de valores de controles internos exigidos pela política.</span><span class="sxs-lookup"><span data-stu-id="0ec15-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="0ec15-117">Valores possíveis: `Block`, `Mfa`, `CompliantDevice` `DomainJoinedDevice`,, `ApprovedApplication`,`CompliantApplication`</span><span class="sxs-lookup"><span data-stu-id="0ec15-117">Possible values: `Block`, `Mfa`, `CompliantDevice`, `DomainJoinedDevice`, `ApprovedApplication`, `CompliantApplication`</span></span> |
| <span data-ttu-id="0ec15-118">customAuthenticationFactors</span><span class="sxs-lookup"><span data-stu-id="0ec15-118">customAuthenticationFactors</span></span> | <span data-ttu-id="0ec15-119">String collection</span><span class="sxs-lookup"><span data-stu-id="0ec15-119">String collection</span></span> | <span data-ttu-id="0ec15-120">Lista de IDs de controles personalizados exigidos pela política.</span><span class="sxs-lookup"><span data-stu-id="0ec15-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="0ec15-121">Saiba mais sobre os controles personalizados aqui:https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span><span class="sxs-lookup"><span data-stu-id="0ec15-121">Learn more about custom controls here: https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span></span> |
| <span data-ttu-id="0ec15-122">termsOfUse</span><span class="sxs-lookup"><span data-stu-id="0ec15-122">termsOfUse</span></span> | <span data-ttu-id="0ec15-123">String collection</span><span class="sxs-lookup"><span data-stu-id="0ec15-123">String collection</span></span> | <span data-ttu-id="0ec15-124">Lista de [termos de uso](agreement.md) IDs exigidos pela política.</span><span class="sxs-lookup"><span data-stu-id="0ec15-124">List of [terms of use](agreement.md) IDs required by the policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0ec15-125">Relações</span><span class="sxs-lookup"><span data-stu-id="0ec15-125">Relationships</span></span>

<span data-ttu-id="0ec15-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0ec15-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ec15-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ec15-127">JSON representation</span></span>

<span data-ttu-id="0ec15-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ec15-128">The following is a JSON representation of the resource.</span></span>

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