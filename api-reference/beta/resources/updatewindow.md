---
title: tipo de recurso updateWindow
description: tipo de recurso updateWindow.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b2aa61d5d815d912caa47fd63d5907b62f882d36
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003448"
---
# <a name="updatewindow-resource-type"></a><span data-ttu-id="f753b-103">tipo de recurso updateWindow</span><span class="sxs-lookup"><span data-stu-id="f753b-103">updateWindow resource type</span></span>

<span data-ttu-id="f753b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f753b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f753b-105">Representa a janela de tempo durante a qual [os agentes](onpremisesagent.md) podem receber atualizações.</span><span class="sxs-lookup"><span data-stu-id="f753b-105">Represents time window during which [agents](onpremisesagent.md) can receive updates.</span></span>

## <a name="properties"></a><span data-ttu-id="f753b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f753b-106">Properties</span></span>

| <span data-ttu-id="f753b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f753b-107">Property</span></span>     | <span data-ttu-id="f753b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f753b-108">Type</span></span>        | <span data-ttu-id="f753b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f753b-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f753b-110">updateWindowEndTime</span><span class="sxs-lookup"><span data-stu-id="f753b-110">updateWindowEndTime</span></span>|<span data-ttu-id="f753b-111">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f753b-111">TimeOfDay</span></span>|<span data-ttu-id="f753b-112">Término de uma janela de tempo durante a qual os agentes podem receber atualizações</span><span class="sxs-lookup"><span data-stu-id="f753b-112">End of a time window during which agents can receive updates</span></span>|
|<span data-ttu-id="f753b-113">updateWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="f753b-113">updateWindowStartTime</span></span>|<span data-ttu-id="f753b-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f753b-114">TimeOfDay</span></span>|<span data-ttu-id="f753b-115">Início de uma janela de tempo durante a qual os agentes podem receber atualizações</span><span class="sxs-lookup"><span data-stu-id="f753b-115">Start of a time window during which agents can receive updates</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f753b-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f753b-116">JSON representation</span></span>

<span data-ttu-id="f753b-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f753b-117">The following is a JSON representation of the resource.</span></span>

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


