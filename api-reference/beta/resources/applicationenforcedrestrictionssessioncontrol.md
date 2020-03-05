---
title: tipo de recurso applicationEnforcedRestrictionsSessionControl
description: Controle de sessão para impor restrições de aplicativo.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b5f608a2915db80d671ab604ab69d256d6aad0ec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508286"
---
# <a name="applicationenforcedrestrictionssessioncontrol-resource-type"></a><span data-ttu-id="fdd1c-103">tipo de recurso applicationEnforcedRestrictionsSessionControl</span><span class="sxs-lookup"><span data-stu-id="fdd1c-103">applicationEnforcedRestrictionsSessionControl resource type</span></span>

<span data-ttu-id="fdd1c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fdd1c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdd1c-105">Controle de sessão para impor restrições de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fdd1c-105">Session control to enforce application restrictions.</span></span> <span data-ttu-id="fdd1c-106">Inehrits do [controle de sessão de acesso condicional](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="fdd1c-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fdd1c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fdd1c-107">Properties</span></span>

| <span data-ttu-id="fdd1c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fdd1c-108">Property</span></span>     | <span data-ttu-id="fdd1c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fdd1c-109">Type</span></span>        | <span data-ttu-id="fdd1c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdd1c-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fdd1c-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="fdd1c-111">isEnabled</span></span>     |<span data-ttu-id="fdd1c-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdd1c-112">Boolean</span></span>      | <span data-ttu-id="fdd1c-113">Especifica se o controle de sessão está habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="fdd1c-113">Specifies whether the session control is enabled or not.</span></span> |

## <a name="relationships"></a><span data-ttu-id="fdd1c-114">Relações</span><span class="sxs-lookup"><span data-stu-id="fdd1c-114">Relationships</span></span>

<span data-ttu-id="fdd1c-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fdd1c-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fdd1c-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fdd1c-116">JSON representation</span></span>

<span data-ttu-id="fdd1c-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fdd1c-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationEnforcedRestrictionsSessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationEnforcedRestrictionsSessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
