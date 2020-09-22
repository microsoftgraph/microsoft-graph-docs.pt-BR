---
title: tipo de recurso callTranscriptionInfo
description: Representa um único evento DTMF.
author: rzhang
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b825264623eb74507e43dcd9302499811377f3fb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069243"
---
# <a name="calltranscriptioninfo-resource-type"></a><span data-ttu-id="406b4-103">tipo de recurso callTranscriptionInfo</span><span class="sxs-lookup"><span data-stu-id="406b4-103">callTranscriptionInfo resource type</span></span>

<span data-ttu-id="406b4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="406b4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="406b4-105">Representa um único evento DTMF.</span><span class="sxs-lookup"><span data-stu-id="406b4-105">Represents a single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="406b4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="406b4-106">Properties</span></span>

| <span data-ttu-id="406b4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="406b4-107">Property</span></span>       | <span data-ttu-id="406b4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="406b4-108">Type</span></span>    | <span data-ttu-id="406b4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="406b4-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="406b4-110">state</span><span class="sxs-lookup"><span data-stu-id="406b4-110">state</span></span> | <span data-ttu-id="406b4-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="406b4-111">String</span></span> | <span data-ttu-id="406b4-112">Os valores possíveis são: `notStarted`, `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="406b4-112">Possible values are: `notStarted`, `active`, `inactive`.</span></span> |
| <span data-ttu-id="406b4-113">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="406b4-113">lastModifiedDateTime</span></span> | <span data-ttu-id="406b4-114">DateTime</span><span class="sxs-lookup"><span data-stu-id="406b4-114">DateTime</span></span> | <span data-ttu-id="406b4-115">O horário de modificação do estado em UTC.</span><span class="sxs-lookup"><span data-stu-id="406b4-115">The state modified time in UTC.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="406b4-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="406b4-116">JSON representation</span></span>

<span data-ttu-id="406b4-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="406b4-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callTranscriptionInfo"
}-->
```json
{
  "state": "notStarted | active | inactive",
  "lastModifiedDateTime": "String (timestamp)"
}
```

