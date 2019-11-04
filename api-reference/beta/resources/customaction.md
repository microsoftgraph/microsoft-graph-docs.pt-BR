---
title: tipo de recurso customAction
description: Representa qualquer ação personalizada que um rótulo pode fornecer, se configurada pelo administrador.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bbb3fc99ce474752fd2382d5777afeb1c56f632e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938867"
---
# <a name="customaction-resource-type"></a><span data-ttu-id="8cde4-103">tipo de recurso customAction</span><span class="sxs-lookup"><span data-stu-id="8cde4-103">customAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cde4-104">Representa qualquer ação personalizada que um rótulo pode fornecer, se configurada pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="8cde4-104">Represents any custom actions that a label may provide, if configured by the administrator.</span></span> <span data-ttu-id="8cde4-105">As ações personalizadas podem ser definidas como parte de um [informationProtectionLabel](informationProtectionLabel.md) por meio do módulo PowerShell do centro de conformidade e segurança do Office 365.</span><span class="sxs-lookup"><span data-stu-id="8cde4-105">Custom actions might be defined as part of an [informationProtectionLabel](informationProtectionLabel.md) via Office 365 Security and Compliance Center's PowerShell module.</span></span> <span data-ttu-id="8cde4-106">As ações devem ser compreendidas pelo aplicativo de consumo.</span><span class="sxs-lookup"><span data-stu-id="8cde4-106">The actions must be understood by the consuming application.</span></span>

## <a name="properties"></a><span data-ttu-id="8cde4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8cde4-107">Properties</span></span>

| <span data-ttu-id="8cde4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8cde4-108">Property</span></span>   | <span data-ttu-id="8cde4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cde4-109">Type</span></span>                                       | <span data-ttu-id="8cde4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cde4-110">Description</span></span>                                          |
| :--------- | :----------------------------------------- | :--------------------------------------------------- |
| <span data-ttu-id="8cde4-111">name</span><span class="sxs-lookup"><span data-stu-id="8cde4-111">name</span></span>       | <span data-ttu-id="8cde4-112">String</span><span class="sxs-lookup"><span data-stu-id="8cde4-112">String</span></span>                                     | <span data-ttu-id="8cde4-113">Nome da ação personalizada.</span><span class="sxs-lookup"><span data-stu-id="8cde4-113">Name of the custom action.</span></span>                           |
| <span data-ttu-id="8cde4-114">properties</span><span class="sxs-lookup"><span data-stu-id="8cde4-114">properties</span></span> | <span data-ttu-id="8cde4-115">Coleção [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="8cde4-115">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="8cde4-116">Propriedades, no formato par de valores chave, da ação.</span><span class="sxs-lookup"><span data-stu-id="8cde4-116">Properties, in key value pair format, of the action.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8cde4-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8cde4-117">JSON representation</span></span>

<span data-ttu-id="8cde4-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8cde4-118">The following is a JSON representation of the resource.</span></span>

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