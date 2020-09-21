---
title: tipo de recurso signInFrequencySessionControl
description: Controle de sessão para impor a frequência de entrada.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8095469ddb29c79be3a22b84e58d7e4e52cd8d5c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067150"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a><span data-ttu-id="4eab5-103">tipo de recurso signInFrequencySessionControl</span><span class="sxs-lookup"><span data-stu-id="4eab5-103">signInFrequencySessionControl resource type</span></span>

<span data-ttu-id="4eab5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4eab5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4eab5-105">Controle de sessão para impor frequência de logon.</span><span class="sxs-lookup"><span data-stu-id="4eab5-105">Session control to enforce sign-in frequency.</span></span> <span data-ttu-id="4eab5-106">Herda do [controle de sessão de acesso condicional](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="4eab5-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4eab5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4eab5-107">Properties</span></span>

| <span data-ttu-id="4eab5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4eab5-108">Property</span></span>     | <span data-ttu-id="4eab5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4eab5-109">Type</span></span>        | <span data-ttu-id="4eab5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4eab5-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4eab5-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="4eab5-111">isEnabled</span></span>     |<span data-ttu-id="4eab5-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="4eab5-112">Boolean</span></span>      | <span data-ttu-id="4eab5-113">Especifica se o controle de sessão está habilitado.</span><span class="sxs-lookup"><span data-stu-id="4eab5-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="4eab5-114">tipo</span><span class="sxs-lookup"><span data-stu-id="4eab5-114">type</span></span>          |<span data-ttu-id="4eab5-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4eab5-115">String</span></span>       | <span data-ttu-id="4eab5-116">Os valores possíveis são: `days` e `hours`.</span><span class="sxs-lookup"><span data-stu-id="4eab5-116">Possible values are: `days`, `hours`.</span></span>|
|<span data-ttu-id="4eab5-117">valor</span><span class="sxs-lookup"><span data-stu-id="4eab5-117">value</span></span>         |<span data-ttu-id="4eab5-118">Int32</span><span class="sxs-lookup"><span data-stu-id="4eab5-118">Int32</span></span>        | <span data-ttu-id="4eab5-119">O número de `days` ou `hours` .</span><span class="sxs-lookup"><span data-stu-id="4eab5-119">The number of `days` or `hours`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4eab5-120">Relações</span><span class="sxs-lookup"><span data-stu-id="4eab5-120">Relationships</span></span>

<span data-ttu-id="4eab5-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4eab5-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4eab5-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4eab5-122">JSON representation</span></span>

<span data-ttu-id="4eab5-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4eab5-123">The following is a JSON representation of the resource.</span></span>

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


