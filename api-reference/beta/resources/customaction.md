---
title: tipo de recurso customAction
description: Representa qualquer ação personalizada que um rótulo pode fornecer, se configurada pelo administrador.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e2a660659f8c0f3a2c6dc571e743884c54365a20
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507321"
---
# <a name="customaction-resource-type"></a><span data-ttu-id="b1587-103">tipo de recurso customAction</span><span class="sxs-lookup"><span data-stu-id="b1587-103">customAction resource type</span></span>

<span data-ttu-id="b1587-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b1587-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1587-105">Representa qualquer ação personalizada que um rótulo pode fornecer, se configurada pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="b1587-105">Represents any custom actions that a label may provide, if configured by the administrator.</span></span> <span data-ttu-id="b1587-106">As ações personalizadas podem ser definidas como parte de um [informationProtectionLabel](informationProtectionLabel.md) por meio do módulo PowerShell do centro de conformidade e segurança do Office 365.</span><span class="sxs-lookup"><span data-stu-id="b1587-106">Custom actions might be defined as part of an [informationProtectionLabel](informationProtectionLabel.md) via Office 365 Security and Compliance Center's PowerShell module.</span></span> <span data-ttu-id="b1587-107">As ações devem ser compreendidas pelo aplicativo de consumo.</span><span class="sxs-lookup"><span data-stu-id="b1587-107">The actions must be understood by the consuming application.</span></span>

## <a name="properties"></a><span data-ttu-id="b1587-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1587-108">Properties</span></span>

| <span data-ttu-id="b1587-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1587-109">Property</span></span>   | <span data-ttu-id="b1587-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1587-110">Type</span></span>                                       | <span data-ttu-id="b1587-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1587-111">Description</span></span>                                          |
| :--------- | :----------------------------------------- | :--------------------------------------------------- |
| <span data-ttu-id="b1587-112">nome</span><span class="sxs-lookup"><span data-stu-id="b1587-112">name</span></span>       | <span data-ttu-id="b1587-113">String</span><span class="sxs-lookup"><span data-stu-id="b1587-113">String</span></span>                                     | <span data-ttu-id="b1587-114">Nome da ação personalizada.</span><span class="sxs-lookup"><span data-stu-id="b1587-114">Name of the custom action.</span></span>                           |
| <span data-ttu-id="b1587-115">properties</span><span class="sxs-lookup"><span data-stu-id="b1587-115">properties</span></span> | <span data-ttu-id="b1587-116">Coleção [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b1587-116">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="b1587-117">Propriedades, no formato par de valores chave, da ação.</span><span class="sxs-lookup"><span data-stu-id="b1587-117">Properties, in key value pair format, of the action.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b1587-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1587-118">JSON representation</span></span>

<span data-ttu-id="b1587-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1587-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.customAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "name": "String",
  "properties": [{"@odata.type": "microsoft.graph.keyValuePair"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "customAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->