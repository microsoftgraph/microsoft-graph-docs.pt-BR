---
title: tipo de recurso callTranscriptionInfo
description: Representa um único evento DTMF.
author: rzhang
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8d4d03d9f01c93113912c1ea7c33f5c92bb31028
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/29/2020
ms.locfileid: "47312177"
---
# <a name="calltranscriptioninfo-resource-type"></a><span data-ttu-id="ff187-103">tipo de recurso callTranscriptionInfo</span><span class="sxs-lookup"><span data-stu-id="ff187-103">callTranscriptionInfo resource type</span></span>

<span data-ttu-id="ff187-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff187-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ff187-105">Representa um único evento DTMF.</span><span class="sxs-lookup"><span data-stu-id="ff187-105">Represents a single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="ff187-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff187-106">Properties</span></span>

| <span data-ttu-id="ff187-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff187-107">Property</span></span>       | <span data-ttu-id="ff187-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff187-108">Type</span></span>    | <span data-ttu-id="ff187-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff187-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ff187-110">estado</span><span class="sxs-lookup"><span data-stu-id="ff187-110">state</span></span> | <span data-ttu-id="ff187-111">String</span><span class="sxs-lookup"><span data-stu-id="ff187-111">String</span></span> | <span data-ttu-id="ff187-112">Os valores possíveis são: `notStarted`, `active`, `inactive`.</span><span class="sxs-lookup"><span data-stu-id="ff187-112">Possible values are: `notStarted`, `active`, `inactive`.</span></span> |
| <span data-ttu-id="ff187-113">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff187-113">lastModifiedDateTime</span></span> | <span data-ttu-id="ff187-114">DateTime</span><span class="sxs-lookup"><span data-stu-id="ff187-114">DateTime</span></span> | <span data-ttu-id="ff187-115">O horário de modificação do estado em UTC.</span><span class="sxs-lookup"><span data-stu-id="ff187-115">The state modified time in UTC.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ff187-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff187-116">JSON representation</span></span>

<span data-ttu-id="ff187-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff187-117">The following is a JSON representation of the resource.</span></span>

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
