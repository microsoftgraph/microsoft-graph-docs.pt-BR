---
title: tipo de recurso modifiedproperty
description: Indica todas as propriedades em um recurso do Azure AD que foram modificadas, incluindo os valores antigo e novo.
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
ms.openlocfilehash: d87d0170dc811db074026e60efc63df928c65ada
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629275"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="0a4ab-103">tipo de recurso modifiedproperty</span><span class="sxs-lookup"><span data-stu-id="0a4ab-103">modifiedProperty resource type</span></span>

<span data-ttu-id="0a4ab-104">Indica todas as propriedades em um recurso do Azure AD que foram modificadas, incluindo os valores antigo e novo.</span><span class="sxs-lookup"><span data-stu-id="0a4ab-104">Indicates all the properties on an Azure AD resource that have been modified, including the old and new values.</span></span>

## <a name="properties"></a><span data-ttu-id="0a4ab-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0a4ab-105">Properties</span></span>

| <span data-ttu-id="0a4ab-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a4ab-106">Property</span></span>     | <span data-ttu-id="0a4ab-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a4ab-107">Type</span></span>   |<span data-ttu-id="0a4ab-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a4ab-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a4ab-109">displayName</span><span class="sxs-lookup"><span data-stu-id="0a4ab-109">displayName</span></span>|<span data-ttu-id="0a4ab-110">String</span><span class="sxs-lookup"><span data-stu-id="0a4ab-110">String</span></span>|<span data-ttu-id="0a4ab-111">Indica o nome da Propriedade do atributo de destino que foi alterado.</span><span class="sxs-lookup"><span data-stu-id="0a4ab-111">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="0a4ab-112">newValue</span><span class="sxs-lookup"><span data-stu-id="0a4ab-112">newValue</span></span>|<span data-ttu-id="0a4ab-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a4ab-113">String</span></span>|<span data-ttu-id="0a4ab-114">Indica o valor atualizado para o correto.</span><span class="sxs-lookup"><span data-stu-id="0a4ab-114">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="0a4ab-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="0a4ab-115">oldValue</span></span>|<span data-ttu-id="0a4ab-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a4ab-116">String</span></span>|<span data-ttu-id="0a4ab-117">Indica o valor anterior (antes da atualização) para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="0a4ab-117">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0a4ab-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0a4ab-118">JSON representation</span></span>

<span data-ttu-id="0a4ab-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0a4ab-119">Here is a JSON representation of the resource.</span></span>

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
