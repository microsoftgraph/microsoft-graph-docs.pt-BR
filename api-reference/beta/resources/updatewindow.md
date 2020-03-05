---
title: tipo de recurso updateWindow
description: tipo de recurso updateWindow.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d0f509accba2cb73709a4a5fa504a5d2a716b038
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519579"
---
# <a name="updatewindow-resource-type"></a><span data-ttu-id="e643f-103">tipo de recurso updateWindow</span><span class="sxs-lookup"><span data-stu-id="e643f-103">updateWindow resource type</span></span>

<span data-ttu-id="e643f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e643f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e643f-105">Representa a janela de tempo durante a qual [os agentes](onpremisesagent.md) podem receber atualizações.</span><span class="sxs-lookup"><span data-stu-id="e643f-105">Represents time window during which [agents](onpremisesagent.md) can receive updates.</span></span>

## <a name="properties"></a><span data-ttu-id="e643f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e643f-106">Properties</span></span>

| <span data-ttu-id="e643f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e643f-107">Property</span></span>     | <span data-ttu-id="e643f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e643f-108">Type</span></span>        | <span data-ttu-id="e643f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e643f-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e643f-110">updateWindowEndTime</span><span class="sxs-lookup"><span data-stu-id="e643f-110">updateWindowEndTime</span></span>|<span data-ttu-id="e643f-111">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="e643f-111">TimeOfDay</span></span>|<span data-ttu-id="e643f-112">Término de uma janela de tempo durante a qual os agentes podem receber atualizações</span><span class="sxs-lookup"><span data-stu-id="e643f-112">End of a time window during which agents can receive updates</span></span>|
|<span data-ttu-id="e643f-113">updateWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="e643f-113">updateWindowStartTime</span></span>|<span data-ttu-id="e643f-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="e643f-114">TimeOfDay</span></span>|<span data-ttu-id="e643f-115">Início de uma janela de tempo durante a qual os agentes podem receber atualizações</span><span class="sxs-lookup"><span data-stu-id="e643f-115">Start of a time window during which agents can receive updates</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e643f-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e643f-116">JSON representation</span></span>

<span data-ttu-id="e643f-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e643f-117">The following is a JSON representation of the resource.</span></span>

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
