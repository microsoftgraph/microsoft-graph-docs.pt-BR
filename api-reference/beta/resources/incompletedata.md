---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
ms.openlocfilehash: add1e3612f65e203f2437419cbb105b78025aa0a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807508"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="76188-102">tipo de recurso de incompleteData</span><span class="sxs-lookup"><span data-stu-id="76188-102">incompleteData resource type</span></span>

 > <span data-ttu-id="76188-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="76188-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76188-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="76188-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="76188-105">A faceta **incompleteData** indica que um recurso foi gerado com dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="76188-105">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="76188-106">As propriedades dentro podem fornecer informações sobre por que não há dados incompletos.</span><span class="sxs-lookup"><span data-stu-id="76188-106">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="76188-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="76188-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="76188-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="76188-108">Properties</span></span>

| <span data-ttu-id="76188-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76188-109">Property</span></span>                  | <span data-ttu-id="76188-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="76188-110">Type</span></span>           | <span data-ttu-id="76188-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="76188-111">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="76188-112">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="76188-112">missingDataBeforeDateTime</span></span> | <span data-ttu-id="76188-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76188-113">DateTimeOffset</span></span> | <span data-ttu-id="76188-114">O serviço não tem dados de origem antes da hora especificada.</span><span class="sxs-lookup"><span data-stu-id="76188-114">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="76188-115">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="76188-115">wasThrottled</span></span>              | <span data-ttu-id="76188-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="76188-116">Boolean</span></span>        | <span data-ttu-id="76188-117">Alguns dados não foi gravados devido à atividade excessiva.</span><span class="sxs-lookup"><span data-stu-id="76188-117">Some data was not recorded due to excessive activity.</span></span>

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData"
} -->
