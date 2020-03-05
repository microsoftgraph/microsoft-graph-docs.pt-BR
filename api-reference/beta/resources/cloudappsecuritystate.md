---
title: tipo de recurso cloudAppSecurityState
description: Contém informações de estado sobre o aplicativo de nuvem (destinationServiceName, destinationServiceIp).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d8e2df4dd25f4209996b4e5cf4f2083790385e84
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507639"
---
# <a name="cloudappsecuritystate-resource-type"></a><span data-ttu-id="7b533-103">tipo de recurso cloudAppSecurityState</span><span class="sxs-lookup"><span data-stu-id="7b533-103">cloudAppSecurityState resource type</span></span>

<span data-ttu-id="7b533-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7b533-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7b533-105">Contém informações de estado sobre o aplicativo de nuvem (destinationServiceName, destinationServiceIp).</span><span class="sxs-lookup"><span data-stu-id="7b533-105">Contains stateful information about the cloud application (destinationServiceName, destinationServiceIp).</span></span>

## <a name="properties"></a><span data-ttu-id="7b533-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b533-106">Properties</span></span>

| <span data-ttu-id="7b533-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b533-107">Property</span></span>     | <span data-ttu-id="7b533-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b533-108">Type</span></span>        | <span data-ttu-id="7b533-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b533-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7b533-110">destinationServiceIp</span><span class="sxs-lookup"><span data-stu-id="7b533-110">destinationServiceIp</span></span>|<span data-ttu-id="7b533-111">String</span><span class="sxs-lookup"><span data-stu-id="7b533-111">String</span></span>|<span data-ttu-id="7b533-112">Endereço IP de destino da conexão com o aplicativo/serviço de nuvem.</span><span class="sxs-lookup"><span data-stu-id="7b533-112">Destination IP Address of the connection to the cloud application/service.</span></span>|
|<span data-ttu-id="7b533-113">destinationServiceName</span><span class="sxs-lookup"><span data-stu-id="7b533-113">destinationServiceName</span></span>|<span data-ttu-id="7b533-114">String</span><span class="sxs-lookup"><span data-stu-id="7b533-114">String</span></span>|<span data-ttu-id="7b533-115">Nome do serviço/aplicativo na nuvem (por exemplo, "Salesforce", "DropBox", etc.).</span><span class="sxs-lookup"><span data-stu-id="7b533-115">Cloud application/service name (for example "Salesforce", "DropBox", etc.).</span></span>|
|<span data-ttu-id="7b533-116">riskScore</span><span class="sxs-lookup"><span data-stu-id="7b533-116">riskScore</span></span>|<span data-ttu-id="7b533-117">String</span><span class="sxs-lookup"><span data-stu-id="7b533-117">String</span></span>|<span data-ttu-id="7b533-118">Pontuação de risco calculado/gerado pelo provedor do aplicativo/serviço de nuvem.</span><span class="sxs-lookup"><span data-stu-id="7b533-118">Provider-generated/calculated risk score of the Cloud Application/Service.</span></span> <span data-ttu-id="7b533-119">O intervalo de valor recomendado de 0-1, que é igual a uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="7b533-119">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b533-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b533-120">JSON representation</span></span>

<span data-ttu-id="7b533-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b533-121">The following is a JSON representation of the resource.</span></span>

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
