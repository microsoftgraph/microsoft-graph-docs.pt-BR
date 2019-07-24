---
title: tipo de recurso updateWindow
description: tipo de recurso updateWindow.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 57fb977dd853261300ed09dd8d9b3c343f62bea0
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840951"
---
# <a name="updatewindow-resource-type"></a><span data-ttu-id="0eb0f-103">tipo de recurso updateWindow</span><span class="sxs-lookup"><span data-stu-id="0eb0f-103">updateWindow resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0eb0f-104">Representa a janela de tempo durante a qual [os agentes](onpremisesagent.md) podem receber atualizações.</span><span class="sxs-lookup"><span data-stu-id="0eb0f-104">Represents time window during which [agents](onpremisesagent.md) can receive updates.</span></span>

## <a name="properties"></a><span data-ttu-id="0eb0f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0eb0f-105">Properties</span></span>

| <span data-ttu-id="0eb0f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0eb0f-106">Property</span></span>     | <span data-ttu-id="0eb0f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="0eb0f-107">Type</span></span>        | <span data-ttu-id="0eb0f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0eb0f-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0eb0f-109">updateWindowEndTime</span><span class="sxs-lookup"><span data-stu-id="0eb0f-109">updateWindowEndTime</span></span>|<span data-ttu-id="0eb0f-110">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="0eb0f-110">TimeOfDay</span></span>|<span data-ttu-id="0eb0f-111">Término de uma janela de tempo durante a qual os agentes podem receber atualizações</span><span class="sxs-lookup"><span data-stu-id="0eb0f-111">End of a time window during which agents can receive updates</span></span>|
|<span data-ttu-id="0eb0f-112">updateWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="0eb0f-112">updateWindowStartTime</span></span>|<span data-ttu-id="0eb0f-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="0eb0f-113">TimeOfDay</span></span>|<span data-ttu-id="0eb0f-114">Início de uma janela de tempo durante a qual os agentes podem receber atualizações</span><span class="sxs-lookup"><span data-stu-id="0eb0f-114">Start of a time window during which agents can receive updates</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0eb0f-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0eb0f-115">JSON representation</span></span>

<span data-ttu-id="0eb0f-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0eb0f-116">The following is a JSON representation of the resource.</span></span>

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
