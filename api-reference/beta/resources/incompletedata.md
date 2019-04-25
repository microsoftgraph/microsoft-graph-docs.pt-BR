---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
ms.openlocfilehash: f2493263d5293b95cbe386b46c56429d11dda089
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549031"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="f50cd-102">tipo de recurso incompleteData</span><span class="sxs-lookup"><span data-stu-id="f50cd-102">incompleteData resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f50cd-103">A faceta **incompleteData** indica que um recurso foi gerado com dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="f50cd-103">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="f50cd-104">As propriedades dentro podem fornecer informações sobre o motivo pelo qual há dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="f50cd-104">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f50cd-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f50cd-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="f50cd-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f50cd-106">Properties</span></span>

| <span data-ttu-id="f50cd-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f50cd-107">Property</span></span>                  | <span data-ttu-id="f50cd-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f50cd-108">Type</span></span>           | <span data-ttu-id="f50cd-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f50cd-109">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="f50cd-110">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="f50cd-110">missingDataBeforeDateTime</span></span> | <span data-ttu-id="f50cd-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f50cd-111">DateTimeOffset</span></span> | <span data-ttu-id="f50cd-112">O serviço não tem dados de origem antes do tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="f50cd-112">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="f50cd-113">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="f50cd-113">wasThrottled</span></span>              | <span data-ttu-id="f50cd-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="f50cd-114">Boolean</span></span>        | <span data-ttu-id="f50cd-115">Alguns dados não foram gravados devido à atividade excessiva.</span><span class="sxs-lookup"><span data-stu-id="f50cd-115">Some data was not recorded due to excessive activity.</span></span>

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": [
    "Error: /api-reference/beta/resources/incompletedata.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
