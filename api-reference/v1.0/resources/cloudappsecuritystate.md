---
title: tipo de recurso cloudAppSecurityState
description: Contém informações de estado sobre o aplicativo de nuvem (destinationServiceName, destinationServiceIp).
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ce08f432b980b110defdfa5a9a7816a71f3f7840
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808260"
---
# <a name="cloudappsecuritystate-resource-type"></a><span data-ttu-id="afd5f-103">tipo de recurso cloudAppSecurityState</span><span class="sxs-lookup"><span data-stu-id="afd5f-103">cloudAppSecurityState resource type</span></span>

<span data-ttu-id="afd5f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afd5f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="afd5f-105">Contém informações de estado sobre o aplicativo de nuvem (destinationServiceName, destinationServiceIp).</span><span class="sxs-lookup"><span data-stu-id="afd5f-105">Contains stateful information about the cloud application (destinationServiceName, destinationServiceIp).</span></span>

## <a name="properties"></a><span data-ttu-id="afd5f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="afd5f-106">Properties</span></span>

| <span data-ttu-id="afd5f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="afd5f-107">Property</span></span>     | <span data-ttu-id="afd5f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="afd5f-108">Type</span></span>        | <span data-ttu-id="afd5f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="afd5f-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="afd5f-110">destinationServiceIp</span><span class="sxs-lookup"><span data-stu-id="afd5f-110">destinationServiceIp</span></span>|<span data-ttu-id="afd5f-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="afd5f-111">String</span></span>|<span data-ttu-id="afd5f-112">Endereço IP de destino da conexão com o aplicativo/serviço de nuvem.</span><span class="sxs-lookup"><span data-stu-id="afd5f-112">Destination IP Address of the connection to the cloud application/service.</span></span>|
|<span data-ttu-id="afd5f-113">destinationServiceName</span><span class="sxs-lookup"><span data-stu-id="afd5f-113">destinationServiceName</span></span>|<span data-ttu-id="afd5f-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="afd5f-114">String</span></span>|<span data-ttu-id="afd5f-115">Nome do serviço/aplicativo na nuvem (por exemplo, "Salesforce", "DropBox", etc.).</span><span class="sxs-lookup"><span data-stu-id="afd5f-115">Cloud application/service name (for example "Salesforce", "DropBox", etc.).</span></span>|
|<span data-ttu-id="afd5f-116">riskScore</span><span class="sxs-lookup"><span data-stu-id="afd5f-116">riskScore</span></span>|<span data-ttu-id="afd5f-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="afd5f-117">String</span></span>|<span data-ttu-id="afd5f-118">Pontuação de risco calculado/gerado pelo provedor do aplicativo/serviço de nuvem.</span><span class="sxs-lookup"><span data-stu-id="afd5f-118">Provider-generated/calculated risk score of the Cloud Application/Service.</span></span> <span data-ttu-id="afd5f-119">O intervalo de valor recomendado de 0-1, que é igual a uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="afd5f-119">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="afd5f-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="afd5f-120">JSON representation</span></span>

<span data-ttu-id="afd5f-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="afd5f-121">The following is a JSON representation of the resource.</span></span>

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
