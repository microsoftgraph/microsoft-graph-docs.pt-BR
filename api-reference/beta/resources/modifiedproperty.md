---
title: tipo de recurso modifiedproperty
description: Descreve as alterações realizadas no sistema de destino.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 78b2447c1bdeab986382ec2d7c5d20787c1f15e2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459794"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="801f8-103">tipo de recurso modifiedproperty</span><span class="sxs-lookup"><span data-stu-id="801f8-103">modifiedProperty resource type</span></span>

<span data-ttu-id="801f8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="801f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="801f8-105">Descreve as alterações realizadas no sistema de destino.</span><span class="sxs-lookup"><span data-stu-id="801f8-105">Describes the changes performed in the target system.</span></span> 

## <a name="properties"></a><span data-ttu-id="801f8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="801f8-106">Properties</span></span>

| <span data-ttu-id="801f8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="801f8-107">Property</span></span>     | <span data-ttu-id="801f8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="801f8-108">Type</span></span>        | <span data-ttu-id="801f8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="801f8-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="801f8-110">displayName</span><span class="sxs-lookup"><span data-stu-id="801f8-110">displayName</span></span>|<span data-ttu-id="801f8-111">String</span><span class="sxs-lookup"><span data-stu-id="801f8-111">String</span></span>|<span data-ttu-id="801f8-112">Nome da propriedade que foi modificada.</span><span class="sxs-lookup"><span data-stu-id="801f8-112">Name of property that was modified.</span></span>|
|<span data-ttu-id="801f8-113">newValue</span><span class="sxs-lookup"><span data-stu-id="801f8-113">newValue</span></span>|<span data-ttu-id="801f8-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="801f8-114">String</span></span>|<span data-ttu-id="801f8-115">Novo valor da propriedade.</span><span class="sxs-lookup"><span data-stu-id="801f8-115">New property value.</span></span>|
|<span data-ttu-id="801f8-116">oldValue</span><span class="sxs-lookup"><span data-stu-id="801f8-116">oldValue</span></span>|<span data-ttu-id="801f8-117">String</span><span class="sxs-lookup"><span data-stu-id="801f8-117">String</span></span>|<span data-ttu-id="801f8-118">Valor da propriedade Old.</span><span class="sxs-lookup"><span data-stu-id="801f8-118">Old property value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="801f8-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="801f8-119">JSON representation</span></span>

<span data-ttu-id="801f8-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="801f8-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.modifiedProperty",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "newValue": "String",
  "oldValue": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "modifiedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
