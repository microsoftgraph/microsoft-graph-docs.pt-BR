---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
ms.openlocfilehash: c951aa05b2b0f6f2b036bdf145e161a8d5b52ba7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544012"
---
# <a name="asyncjobstatus-resource"></a><span data-ttu-id="b09bf-102">Recurso AsyncJobStatus</span><span class="sxs-lookup"><span data-stu-id="b09bf-102">AsyncJobStatus resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b09bf-103">Esse recurso fornece informações sobre o progresso de um trabalho assíncrono.</span><span class="sxs-lookup"><span data-stu-id="b09bf-103">This resource provides information on the status of a asynchronous job progress.</span></span>

<span data-ttu-id="b09bf-104">A seguinte API chama recursos **AsyncJobStatus** de retorno:</span><span class="sxs-lookup"><span data-stu-id="b09bf-104">The following API calls return **AsyncJobStatus** resources:</span></span>

* [<span data-ttu-id="b09bf-105">Copiar item</span><span class="sxs-lookup"><span data-stu-id="b09bf-105">Copy Item</span></span>](../api/driveitem-copy.md)

## <a name="json-representation"></a><span data-ttu-id="b09bf-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b09bf-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a><span data-ttu-id="b09bf-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b09bf-107">Properties</span></span>

| <span data-ttu-id="b09bf-108">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="b09bf-108">Property name</span></span>          | <span data-ttu-id="b09bf-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b09bf-109">Type</span></span>   | <span data-ttu-id="b09bf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b09bf-110">Description</span></span>                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| <span data-ttu-id="b09bf-111">**percentageComplete**</span><span class="sxs-lookup"><span data-stu-id="b09bf-111">**percentageComplete**</span></span> | <span data-ttu-id="b09bf-112">Duplo</span><span class="sxs-lookup"><span data-stu-id="b09bf-112">Double</span></span> | <span data-ttu-id="b09bf-113">Um valor entre 0 e 100 que indica o percentual concluído.</span><span class="sxs-lookup"><span data-stu-id="b09bf-113">A value between 0 and 100 that indicates the percentage complete.</span></span>                          |
| <span data-ttu-id="b09bf-114">**status**</span><span class="sxs-lookup"><span data-stu-id="b09bf-114">**status**</span></span>             | <span data-ttu-id="b09bf-115">String</span><span class="sxs-lookup"><span data-stu-id="b09bf-115">String</span></span> | <span data-ttu-id="b09bf-116">Um valor de cadeia de caracteres que é mapeado para uma enumeração dos valores possíveis sobre o status do trabalho.</span><span class="sxs-lookup"><span data-stu-id="b09bf-116">A string value that maps to an enumeration of possible values about the status of the job.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/beta/resources/asyncjobstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
