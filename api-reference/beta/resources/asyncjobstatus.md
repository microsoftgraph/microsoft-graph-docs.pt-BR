---
author: JeremyKelley
description: Esse recurso fornece informações sobre o status de andamento de um trabalho assíncrono.
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: e8a745a6ab03728eb879767c6af45a423f151d63
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974298"
---
# <a name="asyncjobstatus-resource"></a><span data-ttu-id="4e082-103">Recurso AsyncJobStatus</span><span class="sxs-lookup"><span data-stu-id="4e082-103">AsyncJobStatus resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e082-104">Esse recurso fornece informações sobre o progresso de um trabalho assíncrono.</span><span class="sxs-lookup"><span data-stu-id="4e082-104">This resource provides information on the status of a asynchronous job progress.</span></span>

<span data-ttu-id="4e082-105">A seguinte API chama recursos **AsyncJobStatus** de retorno:</span><span class="sxs-lookup"><span data-stu-id="4e082-105">The following API calls return **AsyncJobStatus** resources:</span></span>

* [<span data-ttu-id="4e082-106">Copiar item</span><span class="sxs-lookup"><span data-stu-id="4e082-106">Copy Item</span></span>](../api/driveitem-copy.md)

## <a name="json-representation"></a><span data-ttu-id="4e082-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4e082-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a><span data-ttu-id="4e082-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4e082-108">Properties</span></span>

| <span data-ttu-id="4e082-109">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="4e082-109">Property name</span></span>          | <span data-ttu-id="4e082-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e082-110">Type</span></span>   | <span data-ttu-id="4e082-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e082-111">Description</span></span>                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| <span data-ttu-id="4e082-112">**percentageComplete**</span><span class="sxs-lookup"><span data-stu-id="4e082-112">**percentageComplete**</span></span> | <span data-ttu-id="4e082-113">Duplo</span><span class="sxs-lookup"><span data-stu-id="4e082-113">Double</span></span> | <span data-ttu-id="4e082-114">Um valor entre 0 e 100 que indica o percentual concluído.</span><span class="sxs-lookup"><span data-stu-id="4e082-114">A value between 0 and 100 that indicates the percentage complete.</span></span>                          |
| <span data-ttu-id="4e082-115">**status**</span><span class="sxs-lookup"><span data-stu-id="4e082-115">**status**</span></span>             | <span data-ttu-id="4e082-116">String</span><span class="sxs-lookup"><span data-stu-id="4e082-116">String</span></span> | <span data-ttu-id="4e082-117">Um valor de cadeia de caracteres que é mapeado para uma enumeração dos valores possíveis sobre o status do trabalho.</span><span class="sxs-lookup"><span data-stu-id="4e082-117">A string value that maps to an enumeration of possible values about the status of the job.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation",
  "suppressions": []
}
-->
