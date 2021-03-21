---
title: Tipo de recurso persistentBrowserSessionControl
description: Controle de sessão para definir se os cookies serão persistentes ou não.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 41e84491593040ff44e9f5097fd6c960f9250b45
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961101"
---
# <a name="persistentbrowsersessioncontrol-resource-type"></a><span data-ttu-id="46fcf-103">Tipo de recurso persistentBrowserSessionControl</span><span class="sxs-lookup"><span data-stu-id="46fcf-103">persistentBrowserSessionControl resource type</span></span>

<span data-ttu-id="46fcf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46fcf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="46fcf-105">Controle de sessão para definir se os cookies serão persistentes ou não.</span><span class="sxs-lookup"><span data-stu-id="46fcf-105">Session control to define whether to persist cookies or not.</span></span> <span data-ttu-id="46fcf-106">Herda do [Controle de Sessão de Acesso Condicional](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="46fcf-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="46fcf-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="46fcf-107">Properties</span></span>

| <span data-ttu-id="46fcf-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46fcf-108">Property</span></span>     | <span data-ttu-id="46fcf-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="46fcf-109">Type</span></span>        | <span data-ttu-id="46fcf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="46fcf-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="46fcf-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="46fcf-111">isEnabled</span></span>     |<span data-ttu-id="46fcf-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="46fcf-112">Boolean</span></span>      | <span data-ttu-id="46fcf-113">Especifica se o controle de sessão está habilitado.</span><span class="sxs-lookup"><span data-stu-id="46fcf-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="46fcf-114">mode</span><span class="sxs-lookup"><span data-stu-id="46fcf-114">mode</span></span>|<span data-ttu-id="46fcf-115">persistentBrowserSessionMode</span><span class="sxs-lookup"><span data-stu-id="46fcf-115">persistentBrowserSessionMode</span></span>| <span data-ttu-id="46fcf-116">Os valores possíveis são: `always`, `never`.</span><span class="sxs-lookup"><span data-stu-id="46fcf-116">Possible values are: `always`, `never`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="46fcf-117">Relações</span><span class="sxs-lookup"><span data-stu-id="46fcf-117">Relationships</span></span>

<span data-ttu-id="46fcf-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="46fcf-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="46fcf-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="46fcf-119">JSON representation</span></span>

<span data-ttu-id="46fcf-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="46fcf-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.persistentBrowserSessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true,
  "mode": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "persistentBrowserSessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

