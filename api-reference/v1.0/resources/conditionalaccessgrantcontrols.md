---
title: tipo de recurso conditionalAccessGrantControls
description: Representa os controles de concessão que devem ser atendidos para passar a política.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aadf38ac5cff15e4c085f77df36aa6fd48fa272f
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384409"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="1f4d6-103">tipo de recurso conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="1f4d6-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="1f4d6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f4d6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1f4d6-105">Representa os controles de concessão que devem ser atendidos para passar a política.</span><span class="sxs-lookup"><span data-stu-id="1f4d6-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="1f4d6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1f4d6-106">Properties</span></span>

| <span data-ttu-id="1f4d6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f4d6-107">Property</span></span> | <span data-ttu-id="1f4d6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f4d6-108">Type</span></span> | <span data-ttu-id="1f4d6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f4d6-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="1f4d6-110">operator</span><span class="sxs-lookup"><span data-stu-id="1f4d6-110">operator</span></span> | <span data-ttu-id="1f4d6-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f4d6-111">String</span></span> | <span data-ttu-id="1f4d6-112">Define o relacionamento dos controles de concessão.</span><span class="sxs-lookup"><span data-stu-id="1f4d6-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="1f4d6-113">Valores possíveis: `AND` , `OR` .</span><span class="sxs-lookup"><span data-stu-id="1f4d6-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="1f4d6-114">builtInControls</span><span class="sxs-lookup"><span data-stu-id="1f4d6-114">builtInControls</span></span> | <span data-ttu-id="1f4d6-115">String collection</span><span class="sxs-lookup"><span data-stu-id="1f4d6-115">String collection</span></span> | <span data-ttu-id="1f4d6-116">Lista de valores de controles internos exigidos pela política.</span><span class="sxs-lookup"><span data-stu-id="1f4d6-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="1f4d6-117">Valores possíveis: `Block` , `Mfa` ,,, `CompliantDevice` `DomainJoinedDevice` `ApprovedApplication` ,`CompliantApplication`</span><span class="sxs-lookup"><span data-stu-id="1f4d6-117">Possible values: `Block`, `Mfa`, `CompliantDevice`, `DomainJoinedDevice`, `ApprovedApplication`, `CompliantApplication`</span></span> |
| <span data-ttu-id="1f4d6-118">customAuthenticationFactors</span><span class="sxs-lookup"><span data-stu-id="1f4d6-118">customAuthenticationFactors</span></span> | <span data-ttu-id="1f4d6-119">String collection</span><span class="sxs-lookup"><span data-stu-id="1f4d6-119">String collection</span></span> | <span data-ttu-id="1f4d6-120">Lista de IDs de controles personalizados exigidos pela política.</span><span class="sxs-lookup"><span data-stu-id="1f4d6-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="1f4d6-121">Para obter mais informações, consulte [Custom Controls](https://docs.microsoft.com/azure/active-directory/conditional-access/controls).</span><span class="sxs-lookup"><span data-stu-id="1f4d6-121">For more information, see [Custom controls](https://docs.microsoft.com/azure/active-directory/conditional-access/controls).</span></span> |
| <span data-ttu-id="1f4d6-122">termsOfUse</span><span class="sxs-lookup"><span data-stu-id="1f4d6-122">termsOfUse</span></span> | <span data-ttu-id="1f4d6-123">String collection</span><span class="sxs-lookup"><span data-stu-id="1f4d6-123">String collection</span></span> | <span data-ttu-id="1f4d6-124">Lista de [termos de uso](https://docs.microsoft.com/graph/api/resources/agreement) IDs exigidos pela política.</span><span class="sxs-lookup"><span data-stu-id="1f4d6-124">List of [terms of use](https://docs.microsoft.com/graph/api/resources/agreement) IDs required by the policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1f4d6-125">Relações</span><span class="sxs-lookup"><span data-stu-id="1f4d6-125">Relationships</span></span>

<span data-ttu-id="1f4d6-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f4d6-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f4d6-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1f4d6-127">JSON representation</span></span>

<span data-ttu-id="1f4d6-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1f4d6-128">The following is a JSON representation of the resource.</span></span>

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
