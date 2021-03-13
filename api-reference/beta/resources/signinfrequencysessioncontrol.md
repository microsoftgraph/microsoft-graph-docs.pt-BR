---
title: Tipo de recurso signInFrequencySessionControl
description: Controle de sessão para impor a frequência de signin.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: bc5123975dc15c7c49f0dcbec507c345cf057850
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761048"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a><span data-ttu-id="e33e6-103">Tipo de recurso signInFrequencySessionControl</span><span class="sxs-lookup"><span data-stu-id="e33e6-103">signInFrequencySessionControl resource type</span></span>

<span data-ttu-id="e33e6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e33e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e33e6-105">Controle de sessão para impor a frequência de login.</span><span class="sxs-lookup"><span data-stu-id="e33e6-105">Session control to enforce sign-in frequency.</span></span> <span data-ttu-id="e33e6-106">Herda do [Controle de Sessão de Acesso Condicional](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="e33e6-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e33e6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e33e6-107">Properties</span></span>

| <span data-ttu-id="e33e6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e33e6-108">Property</span></span>     | <span data-ttu-id="e33e6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e33e6-109">Type</span></span>        | <span data-ttu-id="e33e6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e33e6-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e33e6-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="e33e6-111">isEnabled</span></span>     |<span data-ttu-id="e33e6-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="e33e6-112">Boolean</span></span>      | <span data-ttu-id="e33e6-113">Especifica se o controle de sessão está habilitado.</span><span class="sxs-lookup"><span data-stu-id="e33e6-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="e33e6-114">tipo</span><span class="sxs-lookup"><span data-stu-id="e33e6-114">type</span></span>          |<span data-ttu-id="e33e6-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e33e6-115">String</span></span>       | <span data-ttu-id="e33e6-116">Os valores possíveis são: `days` e `hours`.</span><span class="sxs-lookup"><span data-stu-id="e33e6-116">Possible values are: `days`, `hours`.</span></span>|
|<span data-ttu-id="e33e6-117">valor</span><span class="sxs-lookup"><span data-stu-id="e33e6-117">value</span></span>         |<span data-ttu-id="e33e6-118">Int32</span><span class="sxs-lookup"><span data-stu-id="e33e6-118">Int32</span></span>        | <span data-ttu-id="e33e6-119">O número de `days` ou `hours` .</span><span class="sxs-lookup"><span data-stu-id="e33e6-119">The number of `days` or `hours`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e33e6-120">Relações</span><span class="sxs-lookup"><span data-stu-id="e33e6-120">Relationships</span></span>

<span data-ttu-id="e33e6-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e33e6-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e33e6-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e33e6-122">JSON representation</span></span>

<span data-ttu-id="e33e6-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e33e6-123">The following is a JSON representation of the resource.</span></span>

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


