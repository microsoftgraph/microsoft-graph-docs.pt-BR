---
title: Tipo de recurso detailsInfo
description: Um pacote de propriedades que pode conter qualquer informação sobre a identidade ou sistema associado.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 1841c513651131c4bf624c07ee117fae32df79f7
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240761"
---
# <a name="detailsinfo-resource-type"></a><span data-ttu-id="f67d5-103">Tipo de recurso detailsInfo</span><span class="sxs-lookup"><span data-stu-id="f67d5-103">detailsInfo resource type</span></span>

<span data-ttu-id="f67d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f67d5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f67d5-105">Um pacote de propriedades que pode conter qualquer informação sobre a identidade ou sistema associado.</span><span class="sxs-lookup"><span data-stu-id="f67d5-105">A property bag that can contain any information about the associated identity or system.</span></span> <span data-ttu-id="f67d5-106">Isso pode incluir detalhes sobre a propriedade que está sendo provisionada ou o sistema de origem/destino.</span><span class="sxs-lookup"><span data-stu-id="f67d5-106">This can include details about the property that is being provisioned or the source/target system.</span></span>

## <a name="properties"></a><span data-ttu-id="f67d5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f67d5-107">Properties</span></span>
<span data-ttu-id="f67d5-108">O **recurso detailsInfo** é uma cadeia de caracteres JSON que contém propriedades adicionais, como **ApplicationId,** **ObjectId** e **UPN**.</span><span class="sxs-lookup"><span data-stu-id="f67d5-108">The **detailsInfo** resource is a JSON string that contains additional properties such as **ApplicationId**, **ObjectId**, and **UPN**.</span></span> <span data-ttu-id="f67d5-109">O conjunto de propriedades varia de acordo com o tipo de recurso que está sendo provisionado.</span><span class="sxs-lookup"><span data-stu-id="f67d5-109">The set of properties varies based on the type of resource that is being provisioned.</span></span> <span data-ttu-id="f67d5-110">[A lista provisioningObjectSummary](../api/provisioningobjectsummary-list.md) mostra um exemplo disso.</span><span class="sxs-lookup"><span data-stu-id="f67d5-110">[List provisioningObjectSummary](../api/provisioningobjectsummary-list.md) shows an example of this.</span></span>

## <a name="relationships"></a><span data-ttu-id="f67d5-111">Relações</span><span class="sxs-lookup"><span data-stu-id="f67d5-111">Relationships</span></span>
<span data-ttu-id="f67d5-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f67d5-112">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f67d5-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f67d5-113">JSON Representation</span></span>
<span data-ttu-id="f67d5-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f67d5-114">Here is a JSON representation of the resource.</span></span>
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


