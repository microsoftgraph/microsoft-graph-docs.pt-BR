---
title: tipo de recurso de cloudAppSecurityState
description: Contém informações de estado sobre o aplicativo de nuvem (destinationServiceName, destinationServiceIp).
ms.openlocfilehash: 915044c3084e3d9a9435d602ecc7ec809d2168f2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037566"
---
# <a name="cloudappsecuritystate-resource-type"></a><span data-ttu-id="8c5da-103">tipo de recurso de cloudAppSecurityState</span><span class="sxs-lookup"><span data-stu-id="8c5da-103">cloudAppSecurityState resource type</span></span>

<span data-ttu-id="8c5da-104">Contém informações de estado sobre o aplicativo de nuvem (destinationServiceName, destinationServiceIp).</span><span class="sxs-lookup"><span data-stu-id="8c5da-104">Contains stateful information about the cloud application (destinationServiceName, destinationServiceIp).</span></span>

## <a name="properties"></a><span data-ttu-id="8c5da-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8c5da-105">Properties</span></span>

| <span data-ttu-id="8c5da-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c5da-106">Property</span></span>     | <span data-ttu-id="8c5da-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c5da-107">Type</span></span>        | <span data-ttu-id="8c5da-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c5da-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8c5da-109">destinationServiceIp</span><span class="sxs-lookup"><span data-stu-id="8c5da-109">destinationServiceIp</span></span>|<span data-ttu-id="8c5da-110">String</span><span class="sxs-lookup"><span data-stu-id="8c5da-110">String</span></span>|<span data-ttu-id="8c5da-111">Endereço IP de destino da conexão para o serviço/aplicativo de nuvem.</span><span class="sxs-lookup"><span data-stu-id="8c5da-111">Destination IP Address of the connection to the cloud application/service.</span></span>|
|<span data-ttu-id="8c5da-112">destinationServiceName</span><span class="sxs-lookup"><span data-stu-id="8c5da-112">destinationServiceName</span></span>|<span data-ttu-id="8c5da-113">String</span><span class="sxs-lookup"><span data-stu-id="8c5da-113">String</span></span>|<span data-ttu-id="8c5da-114">Nome do serviço do aplicativo de nuvem (por exemplo "Equipe de vendas", "Recados", etc.).</span><span class="sxs-lookup"><span data-stu-id="8c5da-114">Cloud application/service name (for example "Salesforce", "DropBox", etc.).</span></span>|
|<span data-ttu-id="8c5da-115">riskScore</span><span class="sxs-lookup"><span data-stu-id="8c5da-115">riskScore</span></span>|<span data-ttu-id="8c5da-116">String</span><span class="sxs-lookup"><span data-stu-id="8c5da-116">String</span></span>|<span data-ttu-id="8c5da-117">Pontuação de risco de provedor-gerado/calculado do aplicativo/serviço de nuvem.</span><span class="sxs-lookup"><span data-stu-id="8c5da-117">Provider-generated/calculated risk score of the Cloud Application/Service.</span></span> <span data-ttu-id="8c5da-118">Valor recomendado o intervalo de 0-1, que é igual a um percentual.</span><span class="sxs-lookup"><span data-stu-id="8c5da-118">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8c5da-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8c5da-119">JSON representation</span></span>

<span data-ttu-id="8c5da-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8c5da-120">The following is a JSON representation of the resource.</span></span>

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