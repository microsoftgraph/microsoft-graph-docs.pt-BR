---
title: tipo de recurso de modifiedProperty
description: Indica a todas as propriedades modificadas com valor antigo e o novo valor para qualquer recurso no Azure AD que foi alterado
ms.openlocfilehash: c504969ee12798969aa39490e79cb5b60bdb5435
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035767"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="d85dc-103">tipo de recurso de modifiedProperty</span><span class="sxs-lookup"><span data-stu-id="d85dc-103">modifiedProperty resource type</span></span>
<span data-ttu-id="d85dc-104">Indica a todas as propriedades modificadas com valor antigo e o novo valor para qualquer recurso no Azure AD que foi alterado</span><span class="sxs-lookup"><span data-stu-id="d85dc-104">Indicates all the modified properties with old value and new value for any resource in Azure AD that's changed</span></span>



## <a name="properties"></a><span data-ttu-id="d85dc-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d85dc-105">Properties</span></span>
| <span data-ttu-id="d85dc-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d85dc-106">Property</span></span>     | <span data-ttu-id="d85dc-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d85dc-107">Type</span></span>   |<span data-ttu-id="d85dc-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d85dc-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d85dc-109">displayName</span><span class="sxs-lookup"><span data-stu-id="d85dc-109">displayName</span></span>|<span data-ttu-id="d85dc-110">String</span><span class="sxs-lookup"><span data-stu-id="d85dc-110">String</span></span>|<span data-ttu-id="d85dc-111">Indica o nome da propriedade do atributo-alvo que foi alterado.</span><span class="sxs-lookup"><span data-stu-id="d85dc-111">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="d85dc-112">newValue</span><span class="sxs-lookup"><span data-stu-id="d85dc-112">newValue</span></span>|<span data-ttu-id="d85dc-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d85dc-113">String</span></span>|<span data-ttu-id="d85dc-114">Indica o valor atualizado para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="d85dc-114">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="d85dc-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="d85dc-115">oldValue</span></span>|<span data-ttu-id="d85dc-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d85dc-116">String</span></span>|<span data-ttu-id="d85dc-117">Indica o valor anterior (antes da atualização) para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="d85dc-117">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d85dc-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d85dc-118">JSON representation</span></span>

<span data-ttu-id="d85dc-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d85dc-119">Here is a JSON representation of the resource.</span></span>

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