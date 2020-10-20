---
title: tipo de recurso programResource
description: Representa uma referência a um objeto que é o destino da revisão do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5ad3720587523e6937b4c3713a1c5a8c06d1e6e5
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601493"
---
# <a name="programresource-resource-type"></a><span data-ttu-id="f2be8-103">tipo de recurso programResource</span><span class="sxs-lookup"><span data-stu-id="f2be8-103">programResource resource type</span></span>

<span data-ttu-id="f2be8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2be8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2be8-105">O objeto **programResource** , contido em um objeto [programControl](programcontrol.md) , representa uma referência a um objeto que é o destino da revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="f2be8-105">The **programResource** object, contained within a [programControl](programcontrol.md) object, represents a reference to an object that is the target of the access review.</span></span>

<span data-ttu-id="f2be8-106">Este tipo herda de [Identity](identity.md).</span><span class="sxs-lookup"><span data-stu-id="f2be8-106">This type inherits from [identity](identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f2be8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f2be8-107">Properties</span></span>

| <span data-ttu-id="f2be8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2be8-108">Property</span></span> | <span data-ttu-id="f2be8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2be8-109">Type</span></span> | <span data-ttu-id="f2be8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2be8-110">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="f2be8-111">type</span><span class="sxs-lookup"><span data-stu-id="f2be8-111">type</span></span> | <span data-ttu-id="f2be8-112">String</span><span class="sxs-lookup"><span data-stu-id="f2be8-112">String</span></span> | <span data-ttu-id="f2be8-113">Tipo do recurso, indicando se é um grupo ou um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f2be8-113">Type of the resource, indicating whether it is a group or an app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f2be8-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f2be8-114">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.programResource"
}-->
```json
{
  "type": "string"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "programResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
