---
title: tipo de recurso modifiedproperty
description: Indica todas as propriedades em um recurso do Azure AD que foram modificadas, incluindo os valores antigo e novo.
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
doc_type: resourcePageType
ms.openlocfilehash: 0c5375ea3e188d6023e3588531e07877f6de38ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036096"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="3477a-103">tipo de recurso modifiedproperty</span><span class="sxs-lookup"><span data-stu-id="3477a-103">modifiedProperty resource type</span></span>

<span data-ttu-id="3477a-104">Indica todas as propriedades em um recurso do Azure AD que foram modificadas, incluindo os valores antigo e novo.</span><span class="sxs-lookup"><span data-stu-id="3477a-104">Indicates all the properties on an Azure AD resource that have been modified, including the old and new values.</span></span>

## <a name="properties"></a><span data-ttu-id="3477a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3477a-105">Properties</span></span>

| <span data-ttu-id="3477a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3477a-106">Property</span></span>     | <span data-ttu-id="3477a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3477a-107">Type</span></span>   |<span data-ttu-id="3477a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3477a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3477a-109">displayName</span><span class="sxs-lookup"><span data-stu-id="3477a-109">displayName</span></span>|<span data-ttu-id="3477a-110">String</span><span class="sxs-lookup"><span data-stu-id="3477a-110">String</span></span>|<span data-ttu-id="3477a-111">Indica o nome da Propriedade do atributo de destino que foi alterado.</span><span class="sxs-lookup"><span data-stu-id="3477a-111">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="3477a-112">newValue</span><span class="sxs-lookup"><span data-stu-id="3477a-112">newValue</span></span>|<span data-ttu-id="3477a-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3477a-113">String</span></span>|<span data-ttu-id="3477a-114">Indica o valor atualizado para o correto.</span><span class="sxs-lookup"><span data-stu-id="3477a-114">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="3477a-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="3477a-115">oldValue</span></span>|<span data-ttu-id="3477a-116">String</span><span class="sxs-lookup"><span data-stu-id="3477a-116">String</span></span>|<span data-ttu-id="3477a-117">Indica o valor anterior (antes da atualização) para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="3477a-117">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3477a-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3477a-118">JSON representation</span></span>

<span data-ttu-id="3477a-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3477a-119">Here is a JSON representation of the resource.</span></span>

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
