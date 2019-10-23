---
title: tipo de recurso conditionalAccessGrantControls
description: Representa os controles de concessão que devem ser atendidos para passar a política.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ebeb84ccf0e010ad792133f16f7819ca1d8b8ed0
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638495"
---
# <a name="conditionalaccessgrantcontrols-resource-type"></a><span data-ttu-id="03a3a-103">tipo de recurso conditionalAccessGrantControls</span><span class="sxs-lookup"><span data-stu-id="03a3a-103">conditionalAccessGrantControls resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03a3a-104">Representa os controles de concessão que devem ser atendidos para passar a política.</span><span class="sxs-lookup"><span data-stu-id="03a3a-104">Represents grant controls that must be fulfilled to pass the policy.</span></span>

## <a name="properties"></a><span data-ttu-id="03a3a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="03a3a-105">Properties</span></span>

| <span data-ttu-id="03a3a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03a3a-106">Property</span></span> | <span data-ttu-id="03a3a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="03a3a-107">Type</span></span> | <span data-ttu-id="03a3a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="03a3a-108">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="03a3a-109">operator</span><span class="sxs-lookup"><span data-stu-id="03a3a-109">operator</span></span> | <span data-ttu-id="03a3a-110">String</span><span class="sxs-lookup"><span data-stu-id="03a3a-110">String</span></span> | <span data-ttu-id="03a3a-111">Define o relacionamento dos controles de concessão.</span><span class="sxs-lookup"><span data-stu-id="03a3a-111">Defines the relationship of the grant controls.</span></span> <span data-ttu-id="03a3a-112">Valores possíveis: `AND`, `OR`.</span><span class="sxs-lookup"><span data-stu-id="03a3a-112">Possible values: `AND`, `OR`.</span></span> |
| <span data-ttu-id="03a3a-113">builtInControls</span><span class="sxs-lookup"><span data-stu-id="03a3a-113">builtInControls</span></span> | <span data-ttu-id="03a3a-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="03a3a-114">String collection</span></span> | <span data-ttu-id="03a3a-115">Lista de valores de controles internos exigidos pela política.</span><span class="sxs-lookup"><span data-stu-id="03a3a-115">List of values of built-in controls required by the policy.</span></span> <span data-ttu-id="03a3a-116">Valores possíveis: `Block`, `Mfa`, `CompliantDevice` `DomainJoinedDevice`,, `ApprovedApplication`,`CompliantApplication`</span><span class="sxs-lookup"><span data-stu-id="03a3a-116">Possible values: `Block`, `Mfa`, `CompliantDevice`, `DomainJoinedDevice`, `ApprovedApplication`, `CompliantApplication`</span></span> |
| <span data-ttu-id="03a3a-117">customAuthenticationFactors</span><span class="sxs-lookup"><span data-stu-id="03a3a-117">customAuthenticationFactors</span></span> | <span data-ttu-id="03a3a-118">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="03a3a-118">String collection</span></span> | <span data-ttu-id="03a3a-119">Lista de IDs de controles personalizados exigidos pela política.</span><span class="sxs-lookup"><span data-stu-id="03a3a-119">List of custom controls IDs required by the policy.</span></span> <span data-ttu-id="03a3a-120">Saiba mais sobre os controles personalizados aqui:https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span><span class="sxs-lookup"><span data-stu-id="03a3a-120">Learn more about custom controls here: https://docs.microsoft.com/azure/active-directory/conditional-access/controls#custom-controls-preview</span></span> |
| <span data-ttu-id="03a3a-121">termsOfUse</span><span class="sxs-lookup"><span data-stu-id="03a3a-121">termsOfUse</span></span> | <span data-ttu-id="03a3a-122">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="03a3a-122">String collection</span></span> | <span data-ttu-id="03a3a-123">Lista de [termos de uso](agreement.md) IDs exigidos pela política.</span><span class="sxs-lookup"><span data-stu-id="03a3a-123">List of [terms of use](agreement.md) IDs required by the policy.</span></span> |

## <a name="relationships"></a><span data-ttu-id="03a3a-124">Relações</span><span class="sxs-lookup"><span data-stu-id="03a3a-124">Relationships</span></span>

<span data-ttu-id="03a3a-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="03a3a-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="03a3a-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="03a3a-126">JSON representation</span></span>

<span data-ttu-id="03a3a-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="03a3a-127">The following is a JSON representation of the resource.</span></span>

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