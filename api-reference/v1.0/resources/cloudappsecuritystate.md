---
title: tipo de recurso de cloudAppSecurityState
description: Contém informações de estado sobre o aplicativo de nuvem (destinationServiceName, destinationServiceIp).
localization_priority: Normal
ms.openlocfilehash: ff76adf1d3879c3dac3f19ae122d82c9523d5193
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876801"
---
# <a name="cloudappsecuritystate-resource-type"></a><span data-ttu-id="5a189-103">tipo de recurso de cloudAppSecurityState</span><span class="sxs-lookup"><span data-stu-id="5a189-103">cloudAppSecurityState resource type</span></span>

<span data-ttu-id="5a189-104">Contém informações de estado sobre o aplicativo de nuvem (destinationServiceName, destinationServiceIp).</span><span class="sxs-lookup"><span data-stu-id="5a189-104">Contains stateful information about the cloud application (destinationServiceName, destinationServiceIp).</span></span>

## <a name="properties"></a><span data-ttu-id="5a189-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5a189-105">Properties</span></span>

| <span data-ttu-id="5a189-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a189-106">Property</span></span>     | <span data-ttu-id="5a189-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a189-107">Type</span></span>        | <span data-ttu-id="5a189-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a189-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5a189-109">destinationServiceIp</span><span class="sxs-lookup"><span data-stu-id="5a189-109">destinationServiceIp</span></span>|<span data-ttu-id="5a189-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a189-110">String</span></span>|<span data-ttu-id="5a189-111">Endereço IP de destino da conexão para o serviço/aplicativo de nuvem.</span><span class="sxs-lookup"><span data-stu-id="5a189-111">Destination IP Address of the connection to the cloud application/service.</span></span>|
|<span data-ttu-id="5a189-112">destinationServiceName</span><span class="sxs-lookup"><span data-stu-id="5a189-112">destinationServiceName</span></span>|<span data-ttu-id="5a189-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a189-113">String</span></span>|<span data-ttu-id="5a189-114">Nome do serviço do aplicativo de nuvem (por exemplo "Equipe de vendas", "Recados", etc.).</span><span class="sxs-lookup"><span data-stu-id="5a189-114">Cloud application/service name (for example "Salesforce", "DropBox", etc.).</span></span>|
|<span data-ttu-id="5a189-115">riskScore</span><span class="sxs-lookup"><span data-stu-id="5a189-115">riskScore</span></span>|<span data-ttu-id="5a189-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a189-116">String</span></span>|<span data-ttu-id="5a189-117">Pontuação de risco de provedor-gerado/calculado do aplicativo/serviço de nuvem.</span><span class="sxs-lookup"><span data-stu-id="5a189-117">Provider-generated/calculated risk score of the Cloud Application/Service.</span></span> <span data-ttu-id="5a189-118">Valor recomendado o intervalo de 0-1, que é igual a um percentual.</span><span class="sxs-lookup"><span data-stu-id="5a189-118">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5a189-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a189-119">JSON representation</span></span>

<span data-ttu-id="5a189-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5a189-120">The following is a JSON representation of the resource.</span></span>

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
