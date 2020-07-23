---
title: tipo de recurso applicationEnforcedRestrictionsSessionControl
description: Controle de sessão para impor restrições de aplicativo.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 993b28afafebe1240f99a7eddaeee85e47962ec6
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384457"
---
# <a name="applicationenforcedrestrictionssessioncontrol-resource-type"></a><span data-ttu-id="2006e-103">tipo de recurso applicationEnforcedRestrictionsSessionControl</span><span class="sxs-lookup"><span data-stu-id="2006e-103">applicationEnforcedRestrictionsSessionControl resource type</span></span>

<span data-ttu-id="2006e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2006e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2006e-105">Controle de sessão para impor restrições de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2006e-105">Session control to enforce application restrictions.</span></span> <span data-ttu-id="2006e-106">Herda do [controle de sessão de acesso condicional](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="2006e-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2006e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2006e-107">Properties</span></span>

| <span data-ttu-id="2006e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2006e-108">Property</span></span>     | <span data-ttu-id="2006e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2006e-109">Type</span></span>        | <span data-ttu-id="2006e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2006e-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2006e-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="2006e-111">isEnabled</span></span>     |<span data-ttu-id="2006e-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="2006e-112">Boolean</span></span>      | <span data-ttu-id="2006e-113">Especifica se o controle de sessão está habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="2006e-113">Specifies whether the session control is enabled or not.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2006e-114">Relações</span><span class="sxs-lookup"><span data-stu-id="2006e-114">Relationships</span></span>

<span data-ttu-id="2006e-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2006e-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2006e-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2006e-116">JSON representation</span></span>

<span data-ttu-id="2006e-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2006e-117">The following is a JSON representation of the resource.</span></span>

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
