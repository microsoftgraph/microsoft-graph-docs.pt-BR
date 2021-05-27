---
title: Tipo de recurso provisioningStatusInfo
description: Descreve o status do evento de resumo de provisionamento.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7ab2a67662f6e03fd7f967757a7de7ec92480826
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682058"
---
# <a name="provisioningstatusinfo-resource-type"></a><span data-ttu-id="bad45-103">Tipo de recurso provisioningStatusInfo</span><span class="sxs-lookup"><span data-stu-id="bad45-103">provisioningStatusInfo resource type</span></span>

<span data-ttu-id="bad45-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bad45-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bad45-105">Descreve o status do evento de resumo de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="bad45-105">Describes the status of the provisioning summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="bad45-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bad45-106">Properties</span></span>

| <span data-ttu-id="bad45-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bad45-107">Property</span></span>     | <span data-ttu-id="bad45-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="bad45-108">Type</span></span>        | <span data-ttu-id="bad45-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bad45-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bad45-110">status</span><span class="sxs-lookup"><span data-stu-id="bad45-110">status</span></span>|<span data-ttu-id="bad45-111">String</span><span class="sxs-lookup"><span data-stu-id="bad45-111">String</span></span>| <span data-ttu-id="bad45-112">Os valores possíveis são: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="bad45-112">Possible values are: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="bad45-113">errorInfo</span><span class="sxs-lookup"><span data-stu-id="bad45-113">errorInfo</span></span>|[<span data-ttu-id="bad45-114">provisioningErrorInfo</span><span class="sxs-lookup"><span data-stu-id="bad45-114">provisioningErrorInfo</span></span>](provisioningerrorinfo.md)| <span data-ttu-id="bad45-115">Se o status não for bem-sucedido/ os detalhes ignorados do erro estão contidos nisso.</span><span class="sxs-lookup"><span data-stu-id="bad45-115">If status is not success/ skipped details for the error are contained in this.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bad45-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bad45-116">JSON representation</span></span>

<span data-ttu-id="bad45-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bad45-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningStatusInfo",
  "baseType": null
}-->

```json
{
  "status": "String",
  "errorinfo": {"@odata.type": "microsoft.graph.provisioningErrorInfo"},}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningStatusInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


