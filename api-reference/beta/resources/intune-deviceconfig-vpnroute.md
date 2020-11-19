---
title: tipo de recurso vpnRoute
description: Definição da rota VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7d978b80c79d0cb9f876410e1d2a86723ec55437
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279483"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="1acaf-103">tipo de recurso vpnRoute</span><span class="sxs-lookup"><span data-stu-id="1acaf-103">vpnRoute resource type</span></span>

<span data-ttu-id="1acaf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1acaf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1acaf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1acaf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1acaf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1acaf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1acaf-107">Definição da rota VPN.</span><span class="sxs-lookup"><span data-stu-id="1acaf-107">VPN Route definition.</span></span>

## <a name="properties"></a><span data-ttu-id="1acaf-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1acaf-108">Properties</span></span>
|<span data-ttu-id="1acaf-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1acaf-109">Property</span></span>|<span data-ttu-id="1acaf-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1acaf-110">Type</span></span>|<span data-ttu-id="1acaf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1acaf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1acaf-112">destinationPrefix</span><span class="sxs-lookup"><span data-stu-id="1acaf-112">destinationPrefix</span></span>|<span data-ttu-id="1acaf-113">String</span><span class="sxs-lookup"><span data-stu-id="1acaf-113">String</span></span>|<span data-ttu-id="1acaf-114">Prefixo de destino (endereço IPv4/V6).</span><span class="sxs-lookup"><span data-stu-id="1acaf-114">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="1acaf-115">prefixSize</span><span class="sxs-lookup"><span data-stu-id="1acaf-115">prefixSize</span></span>|<span data-ttu-id="1acaf-116">Int32</span><span class="sxs-lookup"><span data-stu-id="1acaf-116">Int32</span></span>|<span data-ttu-id="1acaf-117">Tamanho do prefixo.</span><span class="sxs-lookup"><span data-stu-id="1acaf-117">Prefix size.</span></span> <span data-ttu-id="1acaf-118">(1-32).</span><span class="sxs-lookup"><span data-stu-id="1acaf-118">(1-32).</span></span> <span data-ttu-id="1acaf-119">Valores válidos de 1 a 32</span><span class="sxs-lookup"><span data-stu-id="1acaf-119">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="1acaf-120">Relações</span><span class="sxs-lookup"><span data-stu-id="1acaf-120">Relationships</span></span>
<span data-ttu-id="1acaf-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1acaf-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1acaf-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1acaf-122">JSON Representation</span></span>
<span data-ttu-id="1acaf-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1acaf-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnRoute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnRoute",
  "destinationPrefix": "String",
  "prefixSize": 1024
}
```




