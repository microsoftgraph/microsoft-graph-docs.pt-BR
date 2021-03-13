---
title: Tipo de recurso statusBase
description: Descreve o status do evento de resumo de provisionamento.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 951ef56ecbe2ff8c2ab9692e4eaa9ddf7811d959
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761020"
---
# <a name="statusbase-resource-type"></a><span data-ttu-id="c79fe-103">Tipo de recurso statusBase</span><span class="sxs-lookup"><span data-stu-id="c79fe-103">statusBase resource type</span></span>

<span data-ttu-id="c79fe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c79fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c79fe-105">Descreve o status do evento de resumo de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="c79fe-105">Describes the status of the provisioning summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="c79fe-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c79fe-106">Properties</span></span>

| <span data-ttu-id="c79fe-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c79fe-107">Property</span></span>     | <span data-ttu-id="c79fe-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c79fe-108">Type</span></span>        | <span data-ttu-id="c79fe-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c79fe-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c79fe-110">status</span><span class="sxs-lookup"><span data-stu-id="c79fe-110">status</span></span>|<span data-ttu-id="c79fe-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c79fe-111">String</span></span>| <span data-ttu-id="c79fe-112">Os valores possíveis são: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c79fe-112">Possible values are: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c79fe-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c79fe-113">JSON representation</span></span>

<span data-ttu-id="c79fe-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c79fe-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.statusBase",
  "baseType": null
}-->

```json
{
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "statusBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


