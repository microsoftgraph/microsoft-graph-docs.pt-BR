---
title: tipo de recurso modifiedproperty
description: Indica todas as propriedades modificadas com o valor antigo e o novo valor de qualquer recurso no Azure AD que foi alterado
localization_priority: Normal
ms.openlocfilehash: 91e5df357a40b2e44bb26edc5fb3bf6965a260e5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506233"
---
# <a name="modifiedproperty-resource-type"></a><span data-ttu-id="498a6-103">tipo de recurso modifiedproperty</span><span class="sxs-lookup"><span data-stu-id="498a6-103">modifiedProperty resource type</span></span>
<span data-ttu-id="498a6-104">Indica todas as propriedades modificadas com o valor antigo e o novo valor de qualquer recurso no Azure AD que foi alterado</span><span class="sxs-lookup"><span data-stu-id="498a6-104">Indicates all the modified properties with old value and new value for any resource in Azure AD that's changed</span></span>



## <a name="properties"></a><span data-ttu-id="498a6-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="498a6-105">Properties</span></span>
| <span data-ttu-id="498a6-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="498a6-106">Property</span></span>     | <span data-ttu-id="498a6-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="498a6-107">Type</span></span>   |<span data-ttu-id="498a6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="498a6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="498a6-109">displayName</span><span class="sxs-lookup"><span data-stu-id="498a6-109">displayName</span></span>|<span data-ttu-id="498a6-110">String</span><span class="sxs-lookup"><span data-stu-id="498a6-110">String</span></span>|<span data-ttu-id="498a6-111">Indica o nome da Propriedade do atributo de destino que foi alterado.</span><span class="sxs-lookup"><span data-stu-id="498a6-111">Indicates the property name of the target attribute that was changed.</span></span>|
|<span data-ttu-id="498a6-112">newValue</span><span class="sxs-lookup"><span data-stu-id="498a6-112">newValue</span></span>|<span data-ttu-id="498a6-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="498a6-113">String</span></span>|<span data-ttu-id="498a6-114">Indica o valor atualizado para o correto.</span><span class="sxs-lookup"><span data-stu-id="498a6-114">Indicates the updated value for the propery.</span></span>|
|<span data-ttu-id="498a6-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="498a6-115">oldValue</span></span>|<span data-ttu-id="498a6-116">String</span><span class="sxs-lookup"><span data-stu-id="498a6-116">String</span></span>|<span data-ttu-id="498a6-117">Indica o valor anterior (antes da atualização) para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="498a6-117">Indicates the previous value (before the update) for the property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="498a6-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="498a6-118">JSON representation</span></span>

<span data-ttu-id="498a6-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="498a6-119">Here is a JSON representation of the resource.</span></span>

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
