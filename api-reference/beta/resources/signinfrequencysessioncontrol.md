---
title: tipo de recurso signInFrequencySessionControl
description: Controle de sessão para impor a frequência de entrada.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ab4eaa619117aa350dcb28be9afd43e1aa2fbc8a
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638775"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a><span data-ttu-id="5d6c2-103">tipo de recurso signInFrequencySessionControl</span><span class="sxs-lookup"><span data-stu-id="5d6c2-103">signInFrequencySessionControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d6c2-104">Controle de sessão para impor frequência de logon.</span><span class="sxs-lookup"><span data-stu-id="5d6c2-104">Session control to enforce sign-in frequency.</span></span> <span data-ttu-id="5d6c2-105">Inehrits do [controle de sessão de acesso condicional](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="5d6c2-105">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5d6c2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5d6c2-106">Properties</span></span>

| <span data-ttu-id="5d6c2-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5d6c2-107">Property</span></span>     | <span data-ttu-id="5d6c2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d6c2-108">Type</span></span>        | <span data-ttu-id="5d6c2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d6c2-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5d6c2-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="5d6c2-110">isEnabled</span></span>     |<span data-ttu-id="5d6c2-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d6c2-111">Boolean</span></span>      | <span data-ttu-id="5d6c2-112">Especifica se o controle de sessão está habilitado.</span><span class="sxs-lookup"><span data-stu-id="5d6c2-112">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="5d6c2-113">type</span><span class="sxs-lookup"><span data-stu-id="5d6c2-113">type</span></span>          |<span data-ttu-id="5d6c2-114">String</span><span class="sxs-lookup"><span data-stu-id="5d6c2-114">String</span></span>       | <span data-ttu-id="5d6c2-115">Os valores possíveis são: `days` e `hours`.</span><span class="sxs-lookup"><span data-stu-id="5d6c2-115">Possible values are: `days`, `hours`.</span></span>|
|<span data-ttu-id="5d6c2-116">valor</span><span class="sxs-lookup"><span data-stu-id="5d6c2-116">value</span></span>         |<span data-ttu-id="5d6c2-117">Int32</span><span class="sxs-lookup"><span data-stu-id="5d6c2-117">Int32</span></span>        | <span data-ttu-id="5d6c2-118">O número de `days` ou `hours`.</span><span class="sxs-lookup"><span data-stu-id="5d6c2-118">The number of `days` or `hours`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d6c2-119">Relações</span><span class="sxs-lookup"><span data-stu-id="5d6c2-119">Relationships</span></span>

<span data-ttu-id="5d6c2-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5d6c2-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d6c2-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5d6c2-121">JSON representation</span></span>

<span data-ttu-id="5d6c2-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5d6c2-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInFrequencySessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true,
  "type": "String",
  "value": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInFrequencySessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->