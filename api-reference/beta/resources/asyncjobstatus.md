---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: AsyncJobStatus
localization_priority: Normal
ms.openlocfilehash: 8c442ad8ff3b23d20e8377a224a3f67b00163f5f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820962"
---
# <a name="asyncjobstatus-resource"></a><span data-ttu-id="ec53c-102">Recurso AsyncJobStatus</span><span class="sxs-lookup"><span data-stu-id="ec53c-102">AsyncJobStatus resource</span></span>

> <span data-ttu-id="ec53c-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ec53c-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec53c-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ec53c-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ec53c-105">Esse recurso fornece informações sobre o progresso de um trabalho assíncrono.</span><span class="sxs-lookup"><span data-stu-id="ec53c-105">This resource provides information on the status of a asynchronous job progress.</span></span>

<span data-ttu-id="ec53c-106">A seguinte API chama recursos **AsyncJobStatus** de retorno:</span><span class="sxs-lookup"><span data-stu-id="ec53c-106">The following API calls return **AsyncJobStatus** resources:</span></span>

* [<span data-ttu-id="ec53c-107">Copiar item</span><span class="sxs-lookup"><span data-stu-id="ec53c-107">Copy Item</span></span>](../api/driveitem-copy.md)

## <a name="json-representation"></a><span data-ttu-id="ec53c-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ec53c-108">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.asyncJobStatus", "@type.aka": "oneDrive.asyncOperationStatus" } -->

```json
{
  "percentageComplete": 100.0,
  "status": "notStarted | inProgress | completed | updating | failed | deletePending | deleteFailed | waiting"
}
```

## <a name="properties"></a><span data-ttu-id="ec53c-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ec53c-109">Properties</span></span>

| <span data-ttu-id="ec53c-110">Nome da propriedade</span><span class="sxs-lookup"><span data-stu-id="ec53c-110">Property name</span></span>          | <span data-ttu-id="ec53c-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec53c-111">Type</span></span>   | <span data-ttu-id="ec53c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec53c-112">Description</span></span>                                                                                |
|:-----------------------|:-------|:-------------------------------------------------------------------------------------------|
| <span data-ttu-id="ec53c-113">**percentageComplete**</span><span class="sxs-lookup"><span data-stu-id="ec53c-113">**percentageComplete**</span></span> | <span data-ttu-id="ec53c-114">Duplo</span><span class="sxs-lookup"><span data-stu-id="ec53c-114">Double</span></span> | <span data-ttu-id="ec53c-115">Um valor entre 0 e 100 que indica o percentual concluído.</span><span class="sxs-lookup"><span data-stu-id="ec53c-115">A value between 0 and 100 that indicates the percentage complete.</span></span>                          |
| <span data-ttu-id="ec53c-116">**status**</span><span class="sxs-lookup"><span data-stu-id="ec53c-116">**status**</span></span>             | <span data-ttu-id="ec53c-117">String</span><span class="sxs-lookup"><span data-stu-id="ec53c-117">String</span></span> | <span data-ttu-id="ec53c-118">Um valor de cadeia de caracteres que é mapeado para uma enumeração dos valores possíveis sobre o status do trabalho.</span><span class="sxs-lookup"><span data-stu-id="ec53c-118">A string value that maps to an enumeration of possible values about the status of the job.</span></span> |

<!-- {
  "type": "#page.annotation",
  "description": "AsyncJobResource provides details about how to poll for an async completion.",
  "keywords": "async,job status,async status,copy,upload from url",
  "section": "documentation"
} -->
