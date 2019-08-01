---
title: tipo de recurso cloudAppSecurityState
description: Contém informações de estado sobre o aplicativo de nuvem (destinationServiceName, destinationServiceIp).
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e000d5d788a293c9aed7b702da2653f42116c0c3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029712"
---
# <a name="cloudappsecuritystate-resource-type"></a><span data-ttu-id="9694a-103">tipo de recurso cloudAppSecurityState</span><span class="sxs-lookup"><span data-stu-id="9694a-103">cloudAppSecurityState resource type</span></span>

<span data-ttu-id="9694a-104">Contém informações de estado sobre o aplicativo de nuvem (destinationServiceName, destinationServiceIp).</span><span class="sxs-lookup"><span data-stu-id="9694a-104">Contains stateful information about the cloud application (destinationServiceName, destinationServiceIp).</span></span>

## <a name="properties"></a><span data-ttu-id="9694a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9694a-105">Properties</span></span>

| <span data-ttu-id="9694a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9694a-106">Property</span></span>     | <span data-ttu-id="9694a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="9694a-107">Type</span></span>        | <span data-ttu-id="9694a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9694a-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9694a-109">destinationServiceIp</span><span class="sxs-lookup"><span data-stu-id="9694a-109">destinationServiceIp</span></span>|<span data-ttu-id="9694a-110">String</span><span class="sxs-lookup"><span data-stu-id="9694a-110">String</span></span>|<span data-ttu-id="9694a-111">Endereço IP de destino da conexão com o aplicativo/serviço de nuvem.</span><span class="sxs-lookup"><span data-stu-id="9694a-111">Destination IP Address of the connection to the cloud application/service.</span></span>|
|<span data-ttu-id="9694a-112">destinationServiceName</span><span class="sxs-lookup"><span data-stu-id="9694a-112">destinationServiceName</span></span>|<span data-ttu-id="9694a-113">String</span><span class="sxs-lookup"><span data-stu-id="9694a-113">String</span></span>|<span data-ttu-id="9694a-114">Nome do serviço/aplicativo na nuvem (por exemplo, "Salesforce", "DropBox", etc.).</span><span class="sxs-lookup"><span data-stu-id="9694a-114">Cloud application/service name (for example "Salesforce", "DropBox", etc.).</span></span>|
|<span data-ttu-id="9694a-115">riskScore</span><span class="sxs-lookup"><span data-stu-id="9694a-115">riskScore</span></span>|<span data-ttu-id="9694a-116">String</span><span class="sxs-lookup"><span data-stu-id="9694a-116">String</span></span>|<span data-ttu-id="9694a-117">Pontuação de risco calculado/gerado pelo provedor do aplicativo/serviço de nuvem.</span><span class="sxs-lookup"><span data-stu-id="9694a-117">Provider-generated/calculated risk score of the Cloud Application/Service.</span></span> <span data-ttu-id="9694a-118">O intervalo de valor recomendado de 0-1, que é igual a uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="9694a-118">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9694a-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9694a-119">JSON representation</span></span>

<span data-ttu-id="9694a-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9694a-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecurityState"
}-->

```json
{
  "destinationServiceIp": "String",
  "destinationServiceName": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
