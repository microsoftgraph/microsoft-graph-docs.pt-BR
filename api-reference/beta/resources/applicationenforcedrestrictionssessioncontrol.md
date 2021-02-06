---
title: Tipo de recurso applicationEnforcedRestrictionsSessionControl
description: Controle de sessão para impor restrições de aplicativo.
localization_priority: Normal
author: sureshja
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f7f20950b3773e660cfc1b0ed4fdec338546e09a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134762"
---
# <a name="applicationenforcedrestrictionssessioncontrol-resource-type"></a><span data-ttu-id="de666-103">Tipo de recurso applicationEnforcedRestrictionsSessionControl</span><span class="sxs-lookup"><span data-stu-id="de666-103">applicationEnforcedRestrictionsSessionControl resource type</span></span>

<span data-ttu-id="de666-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de666-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de666-105">Controle de sessão para impor restrições de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de666-105">Session control to enforce application restrictions.</span></span> <span data-ttu-id="de666-106">Inehrits do [Controle de Sessão de Acesso Condicional.](conditionalaccesssessioncontrol.md)</span><span class="sxs-lookup"><span data-stu-id="de666-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="de666-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="de666-107">Properties</span></span>

| <span data-ttu-id="de666-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de666-108">Property</span></span>     | <span data-ttu-id="de666-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="de666-109">Type</span></span>        | <span data-ttu-id="de666-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="de666-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="de666-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="de666-111">isEnabled</span></span>     |<span data-ttu-id="de666-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="de666-112">Boolean</span></span>      | <span data-ttu-id="de666-113">Especifica se o controle de sessão está habilitado ou não.</span><span class="sxs-lookup"><span data-stu-id="de666-113">Specifies whether the session control is enabled or not.</span></span> |

## <a name="relationships"></a><span data-ttu-id="de666-114">Relações</span><span class="sxs-lookup"><span data-stu-id="de666-114">Relationships</span></span>

<span data-ttu-id="de666-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="de666-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="de666-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="de666-116">JSON representation</span></span>

<span data-ttu-id="de666-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="de666-117">The following is a JSON representation of the resource.</span></span>

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


