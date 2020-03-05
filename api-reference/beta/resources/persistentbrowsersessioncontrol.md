---
title: tipo de recurso persistentBrowserSessionControl
description: Controle de sessão para definir se deseja persistir cookies ou não.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d46ffa5cc3f0eee423b4800ee13f19677bf7c41f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521943"
---
# <a name="persistentbrowsersessioncontrol-resource-type"></a><span data-ttu-id="999a4-103">tipo de recurso persistentBrowserSessionControl</span><span class="sxs-lookup"><span data-stu-id="999a4-103">persistentBrowserSessionControl resource type</span></span>

<span data-ttu-id="999a4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="999a4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="999a4-105">Controle de sessão para definir se deseja persistir cookies ou não.</span><span class="sxs-lookup"><span data-stu-id="999a4-105">Session control to define whether to persist cookies or not.</span></span> <span data-ttu-id="999a4-106">Inehrits do [controle de sessão de acesso condicional](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="999a4-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="999a4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="999a4-107">Properties</span></span>

| <span data-ttu-id="999a4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="999a4-108">Property</span></span>     | <span data-ttu-id="999a4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="999a4-109">Type</span></span>        | <span data-ttu-id="999a4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="999a4-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="999a4-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="999a4-111">isEnabled</span></span>     |<span data-ttu-id="999a4-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="999a4-112">Boolean</span></span>      | <span data-ttu-id="999a4-113">Especifica se o controle de sessão está habilitado.</span><span class="sxs-lookup"><span data-stu-id="999a4-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="999a4-114">Mode</span><span class="sxs-lookup"><span data-stu-id="999a4-114">mode</span></span>|<span data-ttu-id="999a4-115">String</span><span class="sxs-lookup"><span data-stu-id="999a4-115">String</span></span>| <span data-ttu-id="999a4-116">Os valores possíveis são: `always` e `never`.</span><span class="sxs-lookup"><span data-stu-id="999a4-116">Possible values are: `always`, `never`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="999a4-117">Relações</span><span class="sxs-lookup"><span data-stu-id="999a4-117">Relationships</span></span>

<span data-ttu-id="999a4-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="999a4-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="999a4-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="999a4-119">JSON representation</span></span>

<span data-ttu-id="999a4-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="999a4-120">The following is a JSON representation of the resource.</span></span>

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