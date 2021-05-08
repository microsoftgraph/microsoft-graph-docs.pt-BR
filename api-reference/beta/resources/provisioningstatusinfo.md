---
title: Tipo de recurso provisioningStatusInfo
description: Descreve o status do evento de resumo de provisionamento.
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 669201b5527160da6b903614523d633a8c11cb1d
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232902"
---
# <a name="provisioningstatusinfo-resource-type"></a><span data-ttu-id="32b0c-103">Tipo de recurso provisioningStatusInfo</span><span class="sxs-lookup"><span data-stu-id="32b0c-103">provisioningStatusInfo resource type</span></span>

<span data-ttu-id="32b0c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32b0c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32b0c-105">Descreve o status do evento de resumo de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="32b0c-105">Describes the status of the provisioning summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="32b0c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="32b0c-106">Properties</span></span>

| <span data-ttu-id="32b0c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32b0c-107">Property</span></span>     | <span data-ttu-id="32b0c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="32b0c-108">Type</span></span>        | <span data-ttu-id="32b0c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="32b0c-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="32b0c-110">status</span><span class="sxs-lookup"><span data-stu-id="32b0c-110">status</span></span>|<span data-ttu-id="32b0c-111">String</span><span class="sxs-lookup"><span data-stu-id="32b0c-111">String</span></span>| <span data-ttu-id="32b0c-112">Os valores possíveis são: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="32b0c-112">Possible values are: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="32b0c-113">errorInfo</span><span class="sxs-lookup"><span data-stu-id="32b0c-113">errorInfo</span></span>|[<span data-ttu-id="32b0c-114">provisioningErrorInfo</span><span class="sxs-lookup"><span data-stu-id="32b0c-114">provisioningErrorInfo</span></span>](provisioningerrorinfo.md)| <span data-ttu-id="32b0c-115">Se o status não for bem-sucedido/ os detalhes ignorados do erro estão contidos nisso.</span><span class="sxs-lookup"><span data-stu-id="32b0c-115">If status is not success/ skipped details for the error are contained in this.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="32b0c-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="32b0c-116">JSON representation</span></span>

<span data-ttu-id="32b0c-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="32b0c-117">The following is a JSON representation of the resource.</span></span>

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


