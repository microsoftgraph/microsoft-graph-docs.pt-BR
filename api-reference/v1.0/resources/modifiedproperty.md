---
title: Tipo de recurso modifiedProperty
description: Indica todas as propriedades em um recurso do Azure AD que foram modificadas, incluindo os valores antigo e novo.
localization_priority: Normal
author: dhanyahk
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 4e34501f5011310eb7ade73d1c5d938cb58e65cc
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136035"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="f0d38-103">Tipo de recurso modifiedProperty</span><span class="sxs-lookup"><span data-stu-id="f0d38-103">modifiedProperty resource type</span></span>

<span data-ttu-id="f0d38-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0d38-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f0d38-105">Indica todas as propriedades em um recurso do Azure AD que foram modificadas, incluindo os valores antigo e novo.</span><span class="sxs-lookup"><span data-stu-id="f0d38-105">Indicates all the properties on an Azure AD resource that have been modified, including the old and new values.</span></span>

## <a name="properties"></a><span data-ttu-id="f0d38-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0d38-106">Properties</span></span>

| <span data-ttu-id="f0d38-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0d38-107">Property</span></span>     | <span data-ttu-id="f0d38-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0d38-108">Type</span></span>   |<span data-ttu-id="f0d38-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0d38-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0d38-110">displayName</span><span class="sxs-lookup"><span data-stu-id="f0d38-110">displayName</span></span>|<span data-ttu-id="f0d38-111">String</span><span class="sxs-lookup"><span data-stu-id="f0d38-111">String</span></span>|<span data-ttu-id="f0d38-112">Indica o nome da propriedade do atributo de destino que foi alterado.</span><span class="sxs-lookup"><span data-stu-id="f0d38-112">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="f0d38-113">newValue</span><span class="sxs-lookup"><span data-stu-id="f0d38-113">newValue</span></span>|<span data-ttu-id="f0d38-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0d38-114">String</span></span>|<span data-ttu-id="f0d38-115">Indica o valor atualizado para a adequada.</span><span class="sxs-lookup"><span data-stu-id="f0d38-115">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="f0d38-116">oldValue</span><span class="sxs-lookup"><span data-stu-id="f0d38-116">oldValue</span></span>|<span data-ttu-id="f0d38-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0d38-117">String</span></span>|<span data-ttu-id="f0d38-118">Indica o valor anterior (antes da atualização) para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="f0d38-118">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0d38-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0d38-119">JSON representation</span></span>

<span data-ttu-id="f0d38-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f0d38-120">Here is a JSON representation of the resource.</span></span>

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

