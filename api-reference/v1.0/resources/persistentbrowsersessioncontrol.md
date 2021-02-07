---
title: Tipo de recurso persistentBrowserSessionControl
description: Controle de sessão para definir se os cookies serão persistentes ou não.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7b418f16a69e5b97cbb42bc81994dfd87e5a3c1e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135734"
---
# <a name="persistentbrowsersessioncontrol-resource-type"></a><span data-ttu-id="03f9a-103">Tipo de recurso persistentBrowserSessionControl</span><span class="sxs-lookup"><span data-stu-id="03f9a-103">persistentBrowserSessionControl resource type</span></span>

<span data-ttu-id="03f9a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03f9a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="03f9a-105">Controle de sessão para definir se os cookies serão persistentes ou não.</span><span class="sxs-lookup"><span data-stu-id="03f9a-105">Session control to define whether to persist cookies or not.</span></span> <span data-ttu-id="03f9a-106">Herda do [Controle de Sessão de Acesso Condicional.](conditionalaccesssessioncontrol.md)</span><span class="sxs-lookup"><span data-stu-id="03f9a-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="03f9a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="03f9a-107">Properties</span></span>

| <span data-ttu-id="03f9a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03f9a-108">Property</span></span>     | <span data-ttu-id="03f9a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="03f9a-109">Type</span></span>        | <span data-ttu-id="03f9a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="03f9a-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="03f9a-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="03f9a-111">isEnabled</span></span>     |<span data-ttu-id="03f9a-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="03f9a-112">Boolean</span></span>      | <span data-ttu-id="03f9a-113">Especifica se o controle de sessão está habilitado.</span><span class="sxs-lookup"><span data-stu-id="03f9a-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="03f9a-114">modo</span><span class="sxs-lookup"><span data-stu-id="03f9a-114">mode</span></span>|<span data-ttu-id="03f9a-115">String</span><span class="sxs-lookup"><span data-stu-id="03f9a-115">String</span></span>| <span data-ttu-id="03f9a-116">Os valores possíveis são: `always` e `never`.</span><span class="sxs-lookup"><span data-stu-id="03f9a-116">Possible values are: `always`, `never`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03f9a-117">Relações</span><span class="sxs-lookup"><span data-stu-id="03f9a-117">Relationships</span></span>

<span data-ttu-id="03f9a-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="03f9a-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="03f9a-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="03f9a-119">JSON representation</span></span>

<span data-ttu-id="03f9a-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="03f9a-120">The following is a JSON representation of the resource.</span></span>

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

