---
title: tipo de recurso conditionalAccessGrantControls
description: Representa os controles de concessão que devem ser atendidos para passar a política.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9746bfb37dd3887def0f070256d90e46efecbdb6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43413428"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="72f63-103">tipo de recurso conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="72f63-103">conditionalAccessGrantControls resource type</span></span>

<span data-ttu-id="72f63-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72f63-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72f63-105">Representa os controles de concessão que devem ser atendidos para passar a política.</span><span class="sxs-lookup"><span data-stu-id="72f63-105">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="72f63-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="72f63-106">Properties</span></span>

| <span data-ttu-id="72f63-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72f63-107">Property</span></span> | <span data-ttu-id="72f63-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="72f63-108">Type</span></span> | <span data-ttu-id="72f63-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="72f63-109">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="72f63-110">operator</span><span class="sxs-lookup"><span data-stu-id="72f63-110">operator</span></span> | <span data-ttu-id="72f63-111">String</span><span class="sxs-lookup"><span data-stu-id="72f63-111">String</span></span> | <span data-ttu-id="72f63-112">Define o relacionamento dos controles de concessão.</span><span class="sxs-lookup"><span data-stu-id="72f63-112">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="72f63-113">Valores possíveis: `AND`, `OR`.</span><span class="sxs-lookup"><span data-stu-id="72f63-113">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="72f63-114">builtInControls</span><span class="sxs-lookup"><span data-stu-id="72f63-114">builtInControls</span></span> | <span data-ttu-id="72f63-115">Coleção String</span><span class="sxs-lookup"><span data-stu-id="72f63-115">String collection</span></span> | <span data-ttu-id="72f63-116">Lista de valores de controles internos exigidos pela política.</span><span class="sxs-lookup"><span data-stu-id="72f63-116">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="72f63-117">Valores possíveis: `Block`, `Mfa`, `CompliantDevice` `DomainJoinedDevice`,, `ApprovedApplication`,`CompliantApplication`</span><span class="sxs-lookup"><span data-stu-id="72f63-117">Possible values: `Block`, `Mfa`, `CompliantDevice`, `DomainJoinedDevice`, `ApprovedApplication`, `CompliantApplication`</span></span> |
| <span data-ttu-id="72f63-118">customAuthenticationFactors</span><span class="sxs-lookup"><span data-stu-id="72f63-118">customAuthenticationFactors</span></span> | <span data-ttu-id="72f63-119">Coleção String</span><span class="sxs-lookup"><span data-stu-id="72f63-119">String collection</span></span> | <span data-ttu-id="72f63-120">Lista de IDs de controles personalizados exigidos pela política.</span><span class="sxs-lookup"><span data-stu-id="72f63-120">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="72f63-121">Saiba mais sobre os controles personalizados aqui:https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span><span class="sxs-lookup"><span data-stu-id="72f63-121">Learn more about custom controls here: https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span></span> |
| <span data-ttu-id="72f63-122">termsOfUse</span><span class="sxs-lookup"><span data-stu-id="72f63-122">termsOfUse</span></span> | <span data-ttu-id="72f63-123">Coleção String</span><span class="sxs-lookup"><span data-stu-id="72f63-123">String collection</span></span> | <span data-ttu-id="72f63-124">Lista de [termos de uso](agreement.md) IDs exigidos pela política.</span><span class="sxs-lookup"><span data-stu-id="72f63-124">List of [terms of use](agreement.md) IDs required by the policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="72f63-125">Relações</span><span class="sxs-lookup"><span data-stu-id="72f63-125">Relationships</span></span>

<span data-ttu-id="72f63-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="72f63-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="72f63-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="72f63-127">JSON representation</span></span>

<span data-ttu-id="72f63-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="72f63-128">The following is a JSON representation of the resource.</span></span>

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