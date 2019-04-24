---
title: tipo de recurso cloudAppSecurityState
description: Contém informações de estado sobre o aplicativo de nuvem (destinationServiceName, destinationServiceIp).
localization_priority: Normal
ms.openlocfilehash: ff76adf1d3879c3dac3f19ae122d82c9523d5193
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584856"
---
# <a name="cloudappsecuritystate-resource-type"></a><span data-ttu-id="969e6-103">tipo de recurso cloudAppSecurityState</span><span class="sxs-lookup"><span data-stu-id="969e6-103">cloudAppSecurityState resource type</span></span>

<span data-ttu-id="969e6-104">Contém informações de estado sobre o aplicativo de nuvem (destinationServiceName, destinationServiceIp).</span><span class="sxs-lookup"><span data-stu-id="969e6-104">Contains stateful information about the cloud application (destinationServiceName, destinationServiceIp).</span></span>

## <a name="properties"></a><span data-ttu-id="969e6-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="969e6-105">Properties</span></span>

| <span data-ttu-id="969e6-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="969e6-106">Property</span></span>     | <span data-ttu-id="969e6-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="969e6-107">Type</span></span>        | <span data-ttu-id="969e6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="969e6-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="969e6-109">destinationServiceIp</span><span class="sxs-lookup"><span data-stu-id="969e6-109">destinationServiceIp</span></span>|<span data-ttu-id="969e6-110">String</span><span class="sxs-lookup"><span data-stu-id="969e6-110">String</span></span>|<span data-ttu-id="969e6-111">Endereço IP de destino da conexão com o aplicativo/serviço de nuvem.</span><span class="sxs-lookup"><span data-stu-id="969e6-111">Destination IP Address of the connection to the cloud application/service.</span></span>|
|<span data-ttu-id="969e6-112">destinationServiceName</span><span class="sxs-lookup"><span data-stu-id="969e6-112">destinationServiceName</span></span>|<span data-ttu-id="969e6-113">String</span><span class="sxs-lookup"><span data-stu-id="969e6-113">String</span></span>|<span data-ttu-id="969e6-114">Nome do serviço/aplicativo na nuvem (por exemplo, "Salesforce", "DropBox", etc.).</span><span class="sxs-lookup"><span data-stu-id="969e6-114">Cloud application/service name (for example "Salesforce", "DropBox", etc.).</span></span>|
|<span data-ttu-id="969e6-115">riskScore</span><span class="sxs-lookup"><span data-stu-id="969e6-115">riskScore</span></span>|<span data-ttu-id="969e6-116">String</span><span class="sxs-lookup"><span data-stu-id="969e6-116">String</span></span>|<span data-ttu-id="969e6-117">Pontuação de risco calculado/gerado pelo provedor do aplicativo/serviço de nuvem.</span><span class="sxs-lookup"><span data-stu-id="969e6-117">Provider-generated/calculated risk score of the Cloud Application/Service.</span></span> <span data-ttu-id="969e6-118">O intervalo de valor recomendado de 0-1, que é igual a uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="969e6-118">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="969e6-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="969e6-119">JSON representation</span></span>

<span data-ttu-id="969e6-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="969e6-120">The following is a JSON representation of the resource.</span></span>

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
