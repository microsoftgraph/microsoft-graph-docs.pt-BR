---
title: Tipo de recurso signInFrequencySessionControl
description: Controle de sessão para impor a frequência de signin.
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 1f224c1e9ba72e114fd9c9bcacdd74670713837d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945624"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a><span data-ttu-id="65220-103">Tipo de recurso signInFrequencySessionControl</span><span class="sxs-lookup"><span data-stu-id="65220-103">signInFrequencySessionControl resource type</span></span>

<span data-ttu-id="65220-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65220-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65220-105">Controle de sessão para impor a frequência de login.</span><span class="sxs-lookup"><span data-stu-id="65220-105">Session control to enforce sign-in frequency.</span></span> <span data-ttu-id="65220-106">Herda do [Controle de Sessão de Acesso Condicional](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="65220-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="65220-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="65220-107">Properties</span></span>

| <span data-ttu-id="65220-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65220-108">Property</span></span>     | <span data-ttu-id="65220-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="65220-109">Type</span></span>        | <span data-ttu-id="65220-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="65220-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="65220-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="65220-111">isEnabled</span></span>     |<span data-ttu-id="65220-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="65220-112">Boolean</span></span>      | <span data-ttu-id="65220-113">Especifica se o controle de sessão está habilitado.</span><span class="sxs-lookup"><span data-stu-id="65220-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="65220-114">tipo</span><span class="sxs-lookup"><span data-stu-id="65220-114">type</span></span>          |<span data-ttu-id="65220-115">signinFrequencyType</span><span class="sxs-lookup"><span data-stu-id="65220-115">signinFrequencyType</span></span>       | <span data-ttu-id="65220-116">Os valores possíveis são: `days` e `hours`.</span><span class="sxs-lookup"><span data-stu-id="65220-116">Possible values are: `days`, `hours`.</span></span>|
|<span data-ttu-id="65220-117">valor</span><span class="sxs-lookup"><span data-stu-id="65220-117">value</span></span>         |<span data-ttu-id="65220-118">Int32</span><span class="sxs-lookup"><span data-stu-id="65220-118">Int32</span></span>        | <span data-ttu-id="65220-119">O número de `days` ou `hours` .</span><span class="sxs-lookup"><span data-stu-id="65220-119">The number of `days` or `hours`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65220-120">Relações</span><span class="sxs-lookup"><span data-stu-id="65220-120">Relationships</span></span>

<span data-ttu-id="65220-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="65220-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="65220-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="65220-122">JSON representation</span></span>

<span data-ttu-id="65220-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="65220-123">The following is a JSON representation of the resource.</span></span>

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


