---
title: Tipo de recurso updateWindow
description: Tipo de recurso updateWindow.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 7d8f12c7cfcb4c83075087d7b894dc95fe92a695
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761223"
---
# <a name="updatewindow-resource-type"></a><span data-ttu-id="36fd0-103">Tipo de recurso updateWindow</span><span class="sxs-lookup"><span data-stu-id="36fd0-103">updateWindow resource type</span></span>

<span data-ttu-id="36fd0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36fd0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36fd0-105">Representa a janela de tempo durante [a qual os agentes](onpremisesagent.md) podem receber atualizações.</span><span class="sxs-lookup"><span data-stu-id="36fd0-105">Represents time window during which [agents](onpremisesagent.md) can receive updates.</span></span>

## <a name="properties"></a><span data-ttu-id="36fd0-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="36fd0-106">Properties</span></span>

| <span data-ttu-id="36fd0-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36fd0-107">Property</span></span>     | <span data-ttu-id="36fd0-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="36fd0-108">Type</span></span>        | <span data-ttu-id="36fd0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="36fd0-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="36fd0-110">updateWindowEndTime</span><span class="sxs-lookup"><span data-stu-id="36fd0-110">updateWindowEndTime</span></span>|<span data-ttu-id="36fd0-111">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="36fd0-111">TimeOfDay</span></span>|<span data-ttu-id="36fd0-112">Fim de uma janela de tempo durante a qual os agentes podem receber atualizações</span><span class="sxs-lookup"><span data-stu-id="36fd0-112">End of a time window during which agents can receive updates</span></span>|
|<span data-ttu-id="36fd0-113">updateWindowStartTime</span><span class="sxs-lookup"><span data-stu-id="36fd0-113">updateWindowStartTime</span></span>|<span data-ttu-id="36fd0-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="36fd0-114">TimeOfDay</span></span>|<span data-ttu-id="36fd0-115">Início de uma janela de tempo durante a qual os agentes podem receber atualizações</span><span class="sxs-lookup"><span data-stu-id="36fd0-115">Start of a time window during which agents can receive updates</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36fd0-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="36fd0-116">JSON representation</span></span>

<span data-ttu-id="36fd0-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="36fd0-117">The following is a JSON representation of the resource.</span></span>

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


