---
title: tipo de recurso modifiedproperty
description: Descreve as alterações realizadas no sistema de destino.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: dcf55dfc83414b5a516bac6cbeefa3358323b5fd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966689"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="cf11d-103">tipo de recurso modifiedproperty</span><span class="sxs-lookup"><span data-stu-id="cf11d-103">modifiedProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf11d-104">Descreve as alterações realizadas no sistema de destino.</span><span class="sxs-lookup"><span data-stu-id="cf11d-104">Describes the changes performed in the target system.</span></span> 

## <a name="properties"></a><span data-ttu-id="cf11d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf11d-105">Properties</span></span>

| <span data-ttu-id="cf11d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf11d-106">Property</span></span>     | <span data-ttu-id="cf11d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf11d-107">Type</span></span>        | <span data-ttu-id="cf11d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf11d-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cf11d-109">displayName</span><span class="sxs-lookup"><span data-stu-id="cf11d-109">displayName</span></span>|<span data-ttu-id="cf11d-110">String</span><span class="sxs-lookup"><span data-stu-id="cf11d-110">String</span></span>|<span data-ttu-id="cf11d-111">Nome da propriedade que foi modificada.</span><span class="sxs-lookup"><span data-stu-id="cf11d-111">Name of property that was modified.</span></span>|
|<span data-ttu-id="cf11d-112">newValue</span><span class="sxs-lookup"><span data-stu-id="cf11d-112">newValue</span></span>|<span data-ttu-id="cf11d-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cf11d-113">String</span></span>|<span data-ttu-id="cf11d-114">Novo valor da propriedade.</span><span class="sxs-lookup"><span data-stu-id="cf11d-114">New property value.</span></span>|
|<span data-ttu-id="cf11d-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="cf11d-115">oldValue</span></span>|<span data-ttu-id="cf11d-116">String</span><span class="sxs-lookup"><span data-stu-id="cf11d-116">String</span></span>|<span data-ttu-id="cf11d-117">Valor da propriedade Old.</span><span class="sxs-lookup"><span data-stu-id="cf11d-117">Old property value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cf11d-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cf11d-118">JSON representation</span></span>

<span data-ttu-id="cf11d-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cf11d-119">The following is a JSON representation of the resource.</span></span>

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
