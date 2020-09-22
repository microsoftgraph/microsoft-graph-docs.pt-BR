---
title: tipo de recurso modifiedproperty
description: Descreve as alterações realizadas no sistema de destino.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d5dbf7f3ef2078baca54c03e8e67a94f5b52ee85
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021291"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="4d27f-103">tipo de recurso modifiedproperty</span><span class="sxs-lookup"><span data-stu-id="4d27f-103">modifiedProperty resource type</span></span>

<span data-ttu-id="4d27f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d27f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d27f-105">Descreve as alterações realizadas no sistema de destino.</span><span class="sxs-lookup"><span data-stu-id="4d27f-105">Describes the changes performed in the target system.</span></span> 

## <a name="properties"></a><span data-ttu-id="4d27f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4d27f-106">Properties</span></span>

| <span data-ttu-id="4d27f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d27f-107">Property</span></span>     | <span data-ttu-id="4d27f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d27f-108">Type</span></span>        | <span data-ttu-id="4d27f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d27f-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4d27f-110">displayName</span><span class="sxs-lookup"><span data-stu-id="4d27f-110">displayName</span></span>|<span data-ttu-id="4d27f-111">String</span><span class="sxs-lookup"><span data-stu-id="4d27f-111">String</span></span>|<span data-ttu-id="4d27f-112">Nome da propriedade que foi modificada.</span><span class="sxs-lookup"><span data-stu-id="4d27f-112">Name of property that was modified.</span></span>|
|<span data-ttu-id="4d27f-113">newValue</span><span class="sxs-lookup"><span data-stu-id="4d27f-113">newValue</span></span>|<span data-ttu-id="4d27f-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d27f-114">String</span></span>|<span data-ttu-id="4d27f-115">Novo valor da propriedade.</span><span class="sxs-lookup"><span data-stu-id="4d27f-115">New property value.</span></span>|
|<span data-ttu-id="4d27f-116">oldValue</span><span class="sxs-lookup"><span data-stu-id="4d27f-116">oldValue</span></span>|<span data-ttu-id="4d27f-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d27f-117">String</span></span>|<span data-ttu-id="4d27f-118">Valor da propriedade Old.</span><span class="sxs-lookup"><span data-stu-id="4d27f-118">Old property value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4d27f-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4d27f-119">JSON representation</span></span>

<span data-ttu-id="4d27f-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4d27f-120">The following is a JSON representation of the resource.</span></span>

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


