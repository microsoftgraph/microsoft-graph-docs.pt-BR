---
title: tipo de recurso detailsInfo
description: Um conjunto de propriedades que pode conter qualquer informação sobre a identidade ou o sistema associado.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9d3a6726c2151376d858f7962527e4dc6f9b53e7
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349316"
---
# <a name="detailsinfo-resource-type"></a><span data-ttu-id="46dbb-103">tipo de recurso detailsInfo</span><span class="sxs-lookup"><span data-stu-id="46dbb-103">detailsInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46dbb-104">Um conjunto de propriedades que pode conter qualquer informação sobre a identidade ou o sistema associado.</span><span class="sxs-lookup"><span data-stu-id="46dbb-104">A property bag that can contain any information about the associated identity or system.</span></span> <span data-ttu-id="46dbb-105">Isso pode incluir detalhes sobre a propriedade que está sendo provisionada ou o sistema de origem/destino.</span><span class="sxs-lookup"><span data-stu-id="46dbb-105">This can include details about the property that is being provisioned or the source/target system.</span></span>

## <a name="properties"></a><span data-ttu-id="46dbb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="46dbb-106">Properties</span></span>
<span data-ttu-id="46dbb-107">O recurso **detailsInfo** é uma cadeia de caracteres JSON que contém propriedades adicionais como **ApplicationId**, **ObjectID**e **UPN**.</span><span class="sxs-lookup"><span data-stu-id="46dbb-107">The **detailsInfo** resource is a JSON string that contains additional properties such as **ApplicationId**, **ObjectId**, and **UPN**.</span></span> <span data-ttu-id="46dbb-108">O conjunto de propriedades varia com base no tipo de recurso que está sendo provisionado.</span><span class="sxs-lookup"><span data-stu-id="46dbb-108">The set of properties varies based on the type of resource that is being provisioned.</span></span> <span data-ttu-id="46dbb-109">[List provisioningObjectSummary](../api/provisioningobjectsummary-list.md) mostra um exemplo disso.</span><span class="sxs-lookup"><span data-stu-id="46dbb-109">[List provisioningObjectSummary](../api/provisioningobjectsummary-list.md) shows an example of this.</span></span>

## <a name="relationships"></a><span data-ttu-id="46dbb-110">Relações</span><span class="sxs-lookup"><span data-stu-id="46dbb-110">Relationships</span></span>
<span data-ttu-id="46dbb-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="46dbb-111">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="46dbb-112">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="46dbb-112">JSON Representation</span></span>
<span data-ttu-id="46dbb-113">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="46dbb-113">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.detailsInfo",
  "openType": true,
 "optionalProperties": [
 
 ],
}-->
``` json
{
  "@odata.type": "microsoft.graph.detailsInfo"
}
```
