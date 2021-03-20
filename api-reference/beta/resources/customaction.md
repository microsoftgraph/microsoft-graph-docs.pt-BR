---
title: Tipo de recurso customAction
description: Representa todas as ações personalizadas que um rótulo pode fornecer, se configurado pelo administrador.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 1d9c88715cba6fc8faede1419b3c8809c3ec3f54
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941803"
---
# <a name="customaction-resource-type"></a><span data-ttu-id="b9a88-103">Tipo de recurso customAction</span><span class="sxs-lookup"><span data-stu-id="b9a88-103">customAction resource type</span></span>

<span data-ttu-id="b9a88-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9a88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9a88-105">Representa todas as ações personalizadas que um rótulo pode fornecer, se configurado pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="b9a88-105">Represents any custom actions that a label may provide, if configured by the administrator.</span></span> <span data-ttu-id="b9a88-106">Ações personalizadas podem ser definidas como parte de [um informationProtectionLabel](informationProtectionLabel.md) por meio do módulo powerShell do Centro de Conformidade e Segurança do Office 365.</span><span class="sxs-lookup"><span data-stu-id="b9a88-106">Custom actions might be defined as part of an [informationProtectionLabel](informationProtectionLabel.md) via Office 365 Security and Compliance Center's PowerShell module.</span></span> <span data-ttu-id="b9a88-107">As ações devem ser compreendidas pelo aplicativo de consumo.</span><span class="sxs-lookup"><span data-stu-id="b9a88-107">The actions must be understood by the consuming application.</span></span>

## <a name="properties"></a><span data-ttu-id="b9a88-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b9a88-108">Properties</span></span>

| <span data-ttu-id="b9a88-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9a88-109">Property</span></span>   | <span data-ttu-id="b9a88-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9a88-110">Type</span></span>                                       | <span data-ttu-id="b9a88-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9a88-111">Description</span></span>                                          |
| :--------- | :----------------------------------------- | :--------------------------------------------------- |
| <span data-ttu-id="b9a88-112">nome</span><span class="sxs-lookup"><span data-stu-id="b9a88-112">name</span></span>       | <span data-ttu-id="b9a88-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b9a88-113">String</span></span>                                     | <span data-ttu-id="b9a88-114">Nome da ação personalizada.</span><span class="sxs-lookup"><span data-stu-id="b9a88-114">Name of the custom action.</span></span>                           |
| <span data-ttu-id="b9a88-115">properties</span><span class="sxs-lookup"><span data-stu-id="b9a88-115">properties</span></span> | <span data-ttu-id="b9a88-116">Coleção [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="b9a88-116">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="b9a88-117">Propriedades, no formato par de valores-chave, da ação.</span><span class="sxs-lookup"><span data-stu-id="b9a88-117">Properties, in key value pair format, of the action.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b9a88-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b9a88-118">JSON representation</span></span>

<span data-ttu-id="b9a88-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b9a88-119">The following is a JSON representation of the resource.</span></span>

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

