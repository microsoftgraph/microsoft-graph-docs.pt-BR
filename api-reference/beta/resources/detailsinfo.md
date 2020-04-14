---
title: tipo de recurso detailsInfo
description: Um conjunto de propriedades que pode conter qualquer informação sobre a identidade ou o sistema associado.
localization_priority: Normal
author: khotz
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f62a773bb65f5d323ad6f906e53467366f7956d0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463050"
---
# <a name="detailsinfo-resource-type"></a><span data-ttu-id="b163c-103">tipo de recurso detailsInfo</span><span class="sxs-lookup"><span data-stu-id="b163c-103">detailsInfo resource type</span></span>

<span data-ttu-id="b163c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b163c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b163c-105">Um conjunto de propriedades que pode conter qualquer informação sobre a identidade ou o sistema associado.</span><span class="sxs-lookup"><span data-stu-id="b163c-105">A property bag that can contain any information about the associated identity or system.</span></span> <span data-ttu-id="b163c-106">Isso pode incluir detalhes sobre a propriedade que está sendo provisionada ou o sistema de origem/destino.</span><span class="sxs-lookup"><span data-stu-id="b163c-106">This can include details about the property that is being provisioned or the source/target system.</span></span>

## <a name="properties"></a><span data-ttu-id="b163c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b163c-107">Properties</span></span>
<span data-ttu-id="b163c-108">O recurso **detailsInfo** é uma cadeia de caracteres JSON que contém propriedades adicionais como **ApplicationId**, **ObjectID**e **UPN**.</span><span class="sxs-lookup"><span data-stu-id="b163c-108">The **detailsInfo** resource is a JSON string that contains additional properties such as **ApplicationId**, **ObjectId**, and **UPN**.</span></span> <span data-ttu-id="b163c-109">O conjunto de propriedades varia com base no tipo de recurso que está sendo provisionado.</span><span class="sxs-lookup"><span data-stu-id="b163c-109">The set of properties varies based on the type of resource that is being provisioned.</span></span> <span data-ttu-id="b163c-110">[List provisioningObjectSummary](../api/provisioningobjectsummary-list.md) mostra um exemplo disso.</span><span class="sxs-lookup"><span data-stu-id="b163c-110">[List provisioningObjectSummary](../api/provisioningobjectsummary-list.md) shows an example of this.</span></span>

## <a name="relationships"></a><span data-ttu-id="b163c-111">Relações</span><span class="sxs-lookup"><span data-stu-id="b163c-111">Relationships</span></span>
<span data-ttu-id="b163c-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b163c-112">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b163c-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b163c-113">JSON Representation</span></span>
<span data-ttu-id="b163c-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b163c-114">Here is a JSON representation of the resource.</span></span>
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
