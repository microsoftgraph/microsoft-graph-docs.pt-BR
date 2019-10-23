---
title: tipo de recurso persistentBrowserSessionControl
description: Controle de sessão para definir se deseja persistir cookies ou não.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7e2e9304aa8c7e7c8d59602a5710596b14e74636
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638607"
---
# <a name="persistentbrowsersessioncontrol-resource-type"></a><span data-ttu-id="4ff09-103">tipo de recurso persistentBrowserSessionControl</span><span class="sxs-lookup"><span data-stu-id="4ff09-103">persistentBrowserSessionControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ff09-104">Controle de sessão para definir se deseja persistir cookies ou não.</span><span class="sxs-lookup"><span data-stu-id="4ff09-104">Session control to define whether to persist cookies or not.</span></span> <span data-ttu-id="4ff09-105">Inehrits do [controle de sessão de acesso condicional](conditionalaccesssessioncontrol.md).</span><span class="sxs-lookup"><span data-stu-id="4ff09-105">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4ff09-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4ff09-106">Properties</span></span>

| <span data-ttu-id="4ff09-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ff09-107">Property</span></span>     | <span data-ttu-id="4ff09-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ff09-108">Type</span></span>        | <span data-ttu-id="4ff09-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ff09-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4ff09-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="4ff09-110">isEnabled</span></span>     |<span data-ttu-id="4ff09-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ff09-111">Boolean</span></span>      | <span data-ttu-id="4ff09-112">Especifica se o controle de sessão está habilitado.</span><span class="sxs-lookup"><span data-stu-id="4ff09-112">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="4ff09-113">Mode</span><span class="sxs-lookup"><span data-stu-id="4ff09-113">mode</span></span>|<span data-ttu-id="4ff09-114">String</span><span class="sxs-lookup"><span data-stu-id="4ff09-114">String</span></span>| <span data-ttu-id="4ff09-115">Os valores possíveis são: `always` e `never`.</span><span class="sxs-lookup"><span data-stu-id="4ff09-115">Possible values are: `always`, `never`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ff09-116">Relações</span><span class="sxs-lookup"><span data-stu-id="4ff09-116">Relationships</span></span>

<span data-ttu-id="4ff09-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4ff09-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ff09-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ff09-118">JSON representation</span></span>

<span data-ttu-id="4ff09-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4ff09-119">The following is a JSON representation of the resource.</span></span>

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