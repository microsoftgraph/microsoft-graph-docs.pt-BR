---
title: tipo de recurso updateWindow
description: tipo de recurso updateWindow.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a85cef3d3d87ac3b0c4f3bedcb291d6e6c03a054
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43401655"
---
# <a name="updatewindow-resource-type"></a><span data-ttu-id="2436d-103">tipo de recurso updateWindow</span><span class="sxs-lookup"><span data-stu-id="2436d-103">updateWindow resource type</span></span>

<span data-ttu-id="2436d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2436d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2436d-105">Representa a janela de tempo durante a qual [os agentes](onpremisesagent.md) podem receber atualizações.</span><span class="sxs-lookup"><span data-stu-id="2436d-105">Represents time window during which [agents](onpremisesagent.md) can receive updates.</span></span>

## <a name="properties"></a><span data-ttu-id="2436d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2436d-106">Properties</span></span>

| <span data-ttu-id="2436d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2436d-107">Property</span></span>     | <span data-ttu-id="2436d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2436d-108">Type</span></span>        | <span data-ttu-id="2436d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2436d-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2436d-110">updateWindowEndTime</span><span class="sxs-lookup"><span data-stu-id="2436d-110">updateWindowEndTime</span></span>|<span data-ttu-id="2436d-111">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="2436d-111">TimeOfDay</span></span>|<span data-ttu-id="2436d-112">Término de uma janela de tempo durante a qual os agentes podem receber atualizações</span><span class="sxs-lookup"><span data-stu-id="2436d-112">End of a time window during which agents can receive updates</span></span>|
|<span data-ttu-id="2436d-113">updateWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="2436d-113">updateWindowStartTime</span></span>|<span data-ttu-id="2436d-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="2436d-114">TimeOfDay</span></span>|<span data-ttu-id="2436d-115">Início de uma janela de tempo durante a qual os agentes podem receber atualizações</span><span class="sxs-lookup"><span data-stu-id="2436d-115">Start of a time window during which agents can receive updates</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2436d-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2436d-116">JSON representation</span></span>

<span data-ttu-id="2436d-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2436d-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.updateWindow",
  "baseType": null
}-->

```json
{
  "updateWindowEndTime": "String (timestamp)",
  "updateWindowStartTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "updateWindow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
