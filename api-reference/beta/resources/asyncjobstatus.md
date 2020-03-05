---
author: JeremyKelley
description: Esse recurso fornece informações sobre o status de andamento de um trabalho assíncrono.
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 81348ce59e060dadf4201222fca43bf96241dbc3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508168"
---
# <a name="asyncjobstatus-resource"></a><span data-ttu-id="7dbc4-103">Recurso AsyncJobStatus</span><span class="sxs-lookup"><span data-stu-id="7dbc4-103">AsyncJobStatus resource</span></span>

<span data-ttu-id="7dbc4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7dbc4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7dbc4-105">Esse recurso fornece informações sobre o progresso de um trabalho assíncrono.</span><span class="sxs-lookup"><span data-stu-id="7dbc4-105">This resource provides information on the status of a asynchronous job progress.</span></span>

<span data-ttu-id="7dbc4-106">A seguinte API chama recursos **AsyncJobStatus** de retorno:</span><span class="sxs-lookup"><span data-stu-id="7dbc4-106">The following API calls return **AsyncJobStatus** resources:</span></span>

* [<span data-ttu-id="7dbc4-107">Copiar item</span><span class="sxs-lookup"><span data-stu-id="7dbc4-107">Copy Item</span></span>](../api/driveitem-copy.md)

## <a name="json-representation"></a><span data-ttu-id="7dbc4-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7dbc4-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a><span data-ttu-id="7dbc4-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7dbc4-109">Properties</span></span>

| <span data-ttu-id="7dbc4-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="7dbc4-110">Property name</span></span>          | <span data-ttu-id="7dbc4-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="7dbc4-111">Type</span></span>   | <span data-ttu-id="7dbc4-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7dbc4-112">Description</span></span>                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| <span data-ttu-id="7dbc4-113">**percentageComplete**</span><span class="sxs-lookup"><span data-stu-id="7dbc4-113">**percentageComplete**</span></span> | <span data-ttu-id="7dbc4-114">Duplo</span><span class="sxs-lookup"><span data-stu-id="7dbc4-114">Double</span></span> | <span data-ttu-id="7dbc4-115">Um valor entre 0 e 100 que indica o percentual concluído.</span><span class="sxs-lookup"><span data-stu-id="7dbc4-115">A value between 0 and 100 that indicates the percentage complete.</span></span>                          |
| <span data-ttu-id="7dbc4-116">**status**</span><span class="sxs-lookup"><span data-stu-id="7dbc4-116">**status**</span></span>             | <span data-ttu-id="7dbc4-117">String</span><span class="sxs-lookup"><span data-stu-id="7dbc4-117">String</span></span> | <span data-ttu-id="7dbc4-118">Um valor de cadeia de caracteres que é mapeado para uma enumeração dos valores possíveis sobre o status do trabalho.</span><span class="sxs-lookup"><span data-stu-id="7dbc4-118">A string value that maps to an enumeration of possible values about the status of the job.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation",
  "suppressions": []
}
-->
