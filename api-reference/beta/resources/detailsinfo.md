---
title: Tipo de recurso detailsInfo
description: Um pacote de propriedades que pode conter informações sobre a identidade ou o sistema associado.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 25441071581af0b9e35ef941d8c82998bdea7b38
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135650"
---
# <a name="detailsinfo-resource-type"></a><span data-ttu-id="d07a1-103">Tipo de recurso detailsInfo</span><span class="sxs-lookup"><span data-stu-id="d07a1-103">detailsInfo resource type</span></span>

<span data-ttu-id="d07a1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d07a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d07a1-105">Um pacote de propriedades que pode conter informações sobre a identidade ou o sistema associado.</span><span class="sxs-lookup"><span data-stu-id="d07a1-105">A property bag that can contain any information about the associated identity or system.</span></span> <span data-ttu-id="d07a1-106">Isso pode incluir detalhes sobre a propriedade que está sendo provisionada ou o sistema de origem/destino.</span><span class="sxs-lookup"><span data-stu-id="d07a1-106">This can include details about the property that is being provisioned or the source/target system.</span></span>

## <a name="properties"></a><span data-ttu-id="d07a1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d07a1-107">Properties</span></span>
<span data-ttu-id="d07a1-108">O **recurso detailsInfo** é uma cadeia de caracteres JSON que contém propriedades adicionais, como **ApplicationId**, **ObjectId** e **UPN**.</span><span class="sxs-lookup"><span data-stu-id="d07a1-108">The **detailsInfo** resource is a JSON string that contains additional properties such as **ApplicationId**, **ObjectId**, and **UPN**.</span></span> <span data-ttu-id="d07a1-109">O conjunto de propriedades varia com base no tipo de recurso que está sendo provisionado.</span><span class="sxs-lookup"><span data-stu-id="d07a1-109">The set of properties varies based on the type of resource that is being provisioned.</span></span> <span data-ttu-id="d07a1-110">[Listar provisioningObjectSummary](../api/provisioningobjectsummary-list.md) mostra um exemplo disso.</span><span class="sxs-lookup"><span data-stu-id="d07a1-110">[List provisioningObjectSummary](../api/provisioningobjectsummary-list.md) shows an example of this.</span></span>

## <a name="relationships"></a><span data-ttu-id="d07a1-111">Relações</span><span class="sxs-lookup"><span data-stu-id="d07a1-111">Relationships</span></span>
<span data-ttu-id="d07a1-112">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d07a1-112">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d07a1-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d07a1-113">JSON Representation</span></span>
<span data-ttu-id="d07a1-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d07a1-114">Here is a JSON representation of the resource.</span></span>
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


