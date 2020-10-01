---
title: tipo de recurso programResource
description: Representa uma referência a um objeto que é o destino da revisão do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5ad3720587523e6937b4c3713a1c5a8c06d1e6e5
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330414"
---
# <a name="programresource-resource-type"></a><span data-ttu-id="5a084-103">tipo de recurso programResource</span><span class="sxs-lookup"><span data-stu-id="5a084-103">programResource resource type</span></span>

<span data-ttu-id="5a084-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a084-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a084-105">O objeto **programResource** , contido em um objeto [programControl](programcontrol.md) , representa uma referência a um objeto que é o destino da revisão do Access.</span><span class="sxs-lookup"><span data-stu-id="5a084-105">The **programResource** object, contained within a [programControl](programcontrol.md) object, represents a reference to an object that is the target of the access review.</span></span>

<span data-ttu-id="5a084-106">Este tipo herda de [Identity](identity.md).</span><span class="sxs-lookup"><span data-stu-id="5a084-106">This type inherits from [identity](identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5a084-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5a084-107">Properties</span></span>

| <span data-ttu-id="5a084-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a084-108">Property</span></span> | <span data-ttu-id="5a084-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a084-109">Type</span></span> | <span data-ttu-id="5a084-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a084-110">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="5a084-111">tipo</span><span class="sxs-lookup"><span data-stu-id="5a084-111">type</span></span> | <span data-ttu-id="5a084-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a084-112">String</span></span> | <span data-ttu-id="5a084-113">Tipo do recurso, indicando se é um grupo ou um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5a084-113">Type of the resource, indicating whether it is a group or an app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5a084-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a084-114">JSON representation</span></span>

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
