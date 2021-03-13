---
title: Tipo de recurso programResource
description: Representa uma referência a um objeto que é o destino da revisão de acesso.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0ef610650887b1d34569465bd5babb7ec91c194d
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761825"
---
# <a name="programresource-resource-type"></a><span data-ttu-id="6cd8d-103">Tipo de recurso programResource</span><span class="sxs-lookup"><span data-stu-id="6cd8d-103">programResource resource type</span></span>

<span data-ttu-id="6cd8d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cd8d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6cd8d-105">O **objeto programResource,** contido em um objeto [programControl,](programcontrol.md) representa uma referência a um objeto que é o destino da revisão de acesso.</span><span class="sxs-lookup"><span data-stu-id="6cd8d-105">The **programResource** object, contained within a [programControl](programcontrol.md) object, represents a reference to an object that is the target of the access review.</span></span>

<span data-ttu-id="6cd8d-106">Esse tipo herda da [identidade](identity.md).</span><span class="sxs-lookup"><span data-stu-id="6cd8d-106">This type inherits from [identity](identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6cd8d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6cd8d-107">Properties</span></span>

| <span data-ttu-id="6cd8d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6cd8d-108">Property</span></span> | <span data-ttu-id="6cd8d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6cd8d-109">Type</span></span> | <span data-ttu-id="6cd8d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cd8d-110">Description</span></span> |
|:-------- |:---- |:----------- |
| <span data-ttu-id="6cd8d-111">tipo</span><span class="sxs-lookup"><span data-stu-id="6cd8d-111">type</span></span> | <span data-ttu-id="6cd8d-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6cd8d-112">String</span></span> | <span data-ttu-id="6cd8d-113">Tipo do recurso, indicando se é um grupo ou um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cd8d-113">Type of the resource, indicating whether it is a group or an app.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6cd8d-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6cd8d-114">JSON representation</span></span>

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
