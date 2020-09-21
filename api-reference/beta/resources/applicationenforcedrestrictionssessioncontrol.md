---
title: tipo de recurso applicationEnforcedRestrictionsSessionControl
description: Controle de sessão para impor restrições de aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 55e23dead8ea894b57451bf65586672ea125fc35
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050274"
---
# <a name="applicationenforcedrestrictionssessioncontrol-resource-type"></a><span data-ttu-id="df1d8-103">tipo de recurso applicationEnforcedRestrictionsSessionControl</span><span class="sxs-lookup"><span data-stu-id="df1d8-103">applicationEnforcedRestrictionsSessionControl resource type</span></span>

<span data-ttu-id="df1d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df1d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df1d8-105">Controle de sessão para impor restrições de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="df1d8-105">Session control to enforce application restrictions.</span></span> <span data-ttu-id="df1d8-106">Inehrits do [controle de sessão de acesso condicional](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="df1d8-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="df1d8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df1d8-107">Properties</span></span>

| <span data-ttu-id="df1d8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df1d8-108">Property</span></span>     | <span data-ttu-id="df1d8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="df1d8-109">Type</span></span>        | <span data-ttu-id="df1d8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="df1d8-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="df1d8-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="df1d8-111">isEnabled</span></span>     |<span data-ttu-id="df1d8-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="df1d8-112">Boolean</span></span>      | <span data-ttu-id="df1d8-113">Especifica se o controle de sessão está habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="df1d8-113">Specifies whether the session control is enabled or not.</span></span> |

## <a name="relationships"></a><span data-ttu-id="df1d8-114">Relações</span><span class="sxs-lookup"><span data-stu-id="df1d8-114">Relationships</span></span>

<span data-ttu-id="df1d8-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="df1d8-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="df1d8-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="df1d8-116">JSON representation</span></span>

<span data-ttu-id="df1d8-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="df1d8-117">The following is a JSON representation of the resource.</span></span>

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


