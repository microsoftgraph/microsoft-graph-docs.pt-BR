---
title: Tipo de recurso signInFrequencySessionControl
description: Controle de sessão para impor a frequência de signin.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 15255f44971694ff2b815e8f49e1800b91502af3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961927"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a><span data-ttu-id="ad5f0-103">Tipo de recurso signInFrequencySessionControl</span><span class="sxs-lookup"><span data-stu-id="ad5f0-103">signInFrequencySessionControl resource type</span></span>

<span data-ttu-id="ad5f0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad5f0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ad5f0-105">Controle de sessão para impor a frequência de login.</span><span class="sxs-lookup"><span data-stu-id="ad5f0-105">Session control to enforce sign-in frequency.</span></span> <span data-ttu-id="ad5f0-106">Herda do [Controle de Sessão de Acesso Condicional](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="ad5f0-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ad5f0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ad5f0-107">Properties</span></span>

| <span data-ttu-id="ad5f0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ad5f0-108">Property</span></span>     | <span data-ttu-id="ad5f0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ad5f0-109">Type</span></span>        | <span data-ttu-id="ad5f0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ad5f0-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ad5f0-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="ad5f0-111">isEnabled</span></span>     |<span data-ttu-id="ad5f0-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="ad5f0-112">Boolean</span></span>      | <span data-ttu-id="ad5f0-113">Especifica se o controle de sessão está habilitado.</span><span class="sxs-lookup"><span data-stu-id="ad5f0-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="ad5f0-114">tipo</span><span class="sxs-lookup"><span data-stu-id="ad5f0-114">type</span></span>          |<span data-ttu-id="ad5f0-115">signinFrequencyType</span><span class="sxs-lookup"><span data-stu-id="ad5f0-115">signinFrequencyType</span></span>| <span data-ttu-id="ad5f0-116">Os valores possíveis são: `days` e `hours`.</span><span class="sxs-lookup"><span data-stu-id="ad5f0-116">Possible values are: `days`, `hours`.</span></span>|
|<span data-ttu-id="ad5f0-117">valor</span><span class="sxs-lookup"><span data-stu-id="ad5f0-117">value</span></span>         |<span data-ttu-id="ad5f0-118">Int32</span><span class="sxs-lookup"><span data-stu-id="ad5f0-118">Int32</span></span>        | <span data-ttu-id="ad5f0-119">O número de `days` ou `hours` .</span><span class="sxs-lookup"><span data-stu-id="ad5f0-119">The number of `days` or `hours`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad5f0-120">Relações</span><span class="sxs-lookup"><span data-stu-id="ad5f0-120">Relationships</span></span>

<span data-ttu-id="ad5f0-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ad5f0-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad5f0-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ad5f0-122">JSON representation</span></span>

<span data-ttu-id="ad5f0-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ad5f0-123">The following is a JSON representation of the resource.</span></span>

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

