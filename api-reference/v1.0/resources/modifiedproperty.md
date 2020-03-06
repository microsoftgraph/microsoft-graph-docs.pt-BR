---
title: tipo de recurso modifiedproperty
description: Indica todas as propriedades em um recurso do Azure AD que foram modificadas, incluindo os valores antigo e novo.
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
doc_type: resourcePageType
ms.openlocfilehash: 13d377f05650f50f9f87f618ca1c9c07d1da70ee
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534222"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="23e96-103">tipo de recurso modifiedproperty</span><span class="sxs-lookup"><span data-stu-id="23e96-103">modifiedProperty resource type</span></span>

<span data-ttu-id="23e96-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23e96-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="23e96-105">Indica todas as propriedades em um recurso do Azure AD que foram modificadas, incluindo os valores antigo e novo.</span><span class="sxs-lookup"><span data-stu-id="23e96-105">Indicates all the properties on an Azure AD resource that have been modified, including the old and new values.</span></span>

## <a name="properties"></a><span data-ttu-id="23e96-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23e96-106">Properties</span></span>

| <span data-ttu-id="23e96-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23e96-107">Property</span></span>     | <span data-ttu-id="23e96-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="23e96-108">Type</span></span>   |<span data-ttu-id="23e96-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="23e96-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23e96-110">displayName</span><span class="sxs-lookup"><span data-stu-id="23e96-110">displayName</span></span>|<span data-ttu-id="23e96-111">String</span><span class="sxs-lookup"><span data-stu-id="23e96-111">String</span></span>|<span data-ttu-id="23e96-112">Indica o nome da Propriedade do atributo de destino que foi alterado.</span><span class="sxs-lookup"><span data-stu-id="23e96-112">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="23e96-113">newValue</span><span class="sxs-lookup"><span data-stu-id="23e96-113">newValue</span></span>|<span data-ttu-id="23e96-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23e96-114">String</span></span>|<span data-ttu-id="23e96-115">Indica o valor atualizado para o correto.</span><span class="sxs-lookup"><span data-stu-id="23e96-115">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="23e96-116">oldValue</span><span class="sxs-lookup"><span data-stu-id="23e96-116">oldValue</span></span>|<span data-ttu-id="23e96-117">String</span><span class="sxs-lookup"><span data-stu-id="23e96-117">String</span></span>|<span data-ttu-id="23e96-118">Indica o valor anterior (antes da atualização) para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="23e96-118">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="23e96-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23e96-119">JSON representation</span></span>

<span data-ttu-id="23e96-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23e96-120">Here is a JSON representation of the resource.</span></span>

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
