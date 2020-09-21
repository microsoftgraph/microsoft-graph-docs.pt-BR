---
title: tipo de recurso modifiedproperty
description: Indica todas as propriedades em um recurso do Azure AD que foram modificadas, incluindo os valores antigo e novo.
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
doc_type: resourcePageType
ms.openlocfilehash: d98d0aaa4850e8ef2b82f9f5deb17424c3ab98d3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967377"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="95b13-103">tipo de recurso modifiedproperty</span><span class="sxs-lookup"><span data-stu-id="95b13-103">modifiedProperty resource type</span></span>

<span data-ttu-id="95b13-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95b13-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="95b13-105">Indica todas as propriedades em um recurso do Azure AD que foram modificadas, incluindo os valores antigo e novo.</span><span class="sxs-lookup"><span data-stu-id="95b13-105">Indicates all the properties on an Azure AD resource that have been modified, including the old and new values.</span></span>

## <a name="properties"></a><span data-ttu-id="95b13-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="95b13-106">Properties</span></span>

| <span data-ttu-id="95b13-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95b13-107">Property</span></span>     | <span data-ttu-id="95b13-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="95b13-108">Type</span></span>   |<span data-ttu-id="95b13-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="95b13-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95b13-110">displayName</span><span class="sxs-lookup"><span data-stu-id="95b13-110">displayName</span></span>|<span data-ttu-id="95b13-111">String</span><span class="sxs-lookup"><span data-stu-id="95b13-111">String</span></span>|<span data-ttu-id="95b13-112">Indica o nome da Propriedade do atributo de destino que foi alterado.</span><span class="sxs-lookup"><span data-stu-id="95b13-112">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="95b13-113">newValue</span><span class="sxs-lookup"><span data-stu-id="95b13-113">newValue</span></span>|<span data-ttu-id="95b13-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="95b13-114">String</span></span>|<span data-ttu-id="95b13-115">Indica o valor atualizado para o correto.</span><span class="sxs-lookup"><span data-stu-id="95b13-115">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="95b13-116">oldValue</span><span class="sxs-lookup"><span data-stu-id="95b13-116">oldValue</span></span>|<span data-ttu-id="95b13-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="95b13-117">String</span></span>|<span data-ttu-id="95b13-118">Indica o valor anterior (antes da atualização) para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="95b13-118">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="95b13-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="95b13-119">JSON representation</span></span>

<span data-ttu-id="95b13-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="95b13-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.modifiedProperty"
}-->

```json
{
  "displayName": "String",
  "newValue": "String",
  "oldValue": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "modifiedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

