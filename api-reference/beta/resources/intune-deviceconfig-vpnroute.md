---
title: tipo de recurso vpnRoute
description: Definição da rota VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5d3f5d88c7deff5d026f6fe853cf85aa1484becb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728304"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="8cc2b-103">tipo de recurso vpnRoute</span><span class="sxs-lookup"><span data-stu-id="8cc2b-103">vpnRoute resource type</span></span>

<span data-ttu-id="8cc2b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cc2b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8cc2b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8cc2b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cc2b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8cc2b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cc2b-107">Definição da rota VPN.</span><span class="sxs-lookup"><span data-stu-id="8cc2b-107">VPN Route definition.</span></span>

## <a name="properties"></a><span data-ttu-id="8cc2b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8cc2b-108">Properties</span></span>
|<span data-ttu-id="8cc2b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8cc2b-109">Property</span></span>|<span data-ttu-id="8cc2b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cc2b-110">Type</span></span>|<span data-ttu-id="8cc2b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cc2b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cc2b-112">destinationPrefix</span><span class="sxs-lookup"><span data-stu-id="8cc2b-112">destinationPrefix</span></span>|<span data-ttu-id="8cc2b-113">String</span><span class="sxs-lookup"><span data-stu-id="8cc2b-113">String</span></span>|<span data-ttu-id="8cc2b-114">Prefixo de destino (endereço IPv4/V6).</span><span class="sxs-lookup"><span data-stu-id="8cc2b-114">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="8cc2b-115">prefixSize</span><span class="sxs-lookup"><span data-stu-id="8cc2b-115">prefixSize</span></span>|<span data-ttu-id="8cc2b-116">Int32</span><span class="sxs-lookup"><span data-stu-id="8cc2b-116">Int32</span></span>|<span data-ttu-id="8cc2b-117">Tamanho do prefixo.</span><span class="sxs-lookup"><span data-stu-id="8cc2b-117">Prefix size.</span></span> <span data-ttu-id="8cc2b-118">(1-32).</span><span class="sxs-lookup"><span data-stu-id="8cc2b-118">(1-32).</span></span> <span data-ttu-id="8cc2b-119">Valores válidos de 1 a 32</span><span class="sxs-lookup"><span data-stu-id="8cc2b-119">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cc2b-120">Relações</span><span class="sxs-lookup"><span data-stu-id="8cc2b-120">Relationships</span></span>
<span data-ttu-id="8cc2b-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8cc2b-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8cc2b-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8cc2b-122">JSON Representation</span></span>
<span data-ttu-id="8cc2b-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8cc2b-123">Here is a JSON representation of the resource.</span></span>
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





