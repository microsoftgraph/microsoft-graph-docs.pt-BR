---
title: tipo de recurso vpnRoute
description: Definição da rota VPN.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1ee8e52bb838a688f11d4242ce85241fe0c06122
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420322"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="40a23-103">tipo de recurso vpnRoute</span><span class="sxs-lookup"><span data-stu-id="40a23-103">vpnRoute resource type</span></span>

<span data-ttu-id="40a23-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40a23-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="40a23-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="40a23-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40a23-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="40a23-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40a23-107">Definição da rota VPN.</span><span class="sxs-lookup"><span data-stu-id="40a23-107">VPN Route definition.</span></span>

## <a name="properties"></a><span data-ttu-id="40a23-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="40a23-108">Properties</span></span>
|<span data-ttu-id="40a23-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40a23-109">Property</span></span>|<span data-ttu-id="40a23-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="40a23-110">Type</span></span>|<span data-ttu-id="40a23-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="40a23-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40a23-112">destinationPrefix</span><span class="sxs-lookup"><span data-stu-id="40a23-112">destinationPrefix</span></span>|<span data-ttu-id="40a23-113">String</span><span class="sxs-lookup"><span data-stu-id="40a23-113">String</span></span>|<span data-ttu-id="40a23-114">Prefixo de destino (endereço IPv4/V6).</span><span class="sxs-lookup"><span data-stu-id="40a23-114">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="40a23-115">prefixSize</span><span class="sxs-lookup"><span data-stu-id="40a23-115">prefixSize</span></span>|<span data-ttu-id="40a23-116">Int32</span><span class="sxs-lookup"><span data-stu-id="40a23-116">Int32</span></span>|<span data-ttu-id="40a23-117">Tamanho do prefixo.</span><span class="sxs-lookup"><span data-stu-id="40a23-117">Prefix size.</span></span> <span data-ttu-id="40a23-118">(1-32).</span><span class="sxs-lookup"><span data-stu-id="40a23-118">(1-32).</span></span> <span data-ttu-id="40a23-119">Valores válidos de 1 a 32</span><span class="sxs-lookup"><span data-stu-id="40a23-119">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="40a23-120">Relações</span><span class="sxs-lookup"><span data-stu-id="40a23-120">Relationships</span></span>
<span data-ttu-id="40a23-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="40a23-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="40a23-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="40a23-122">JSON Representation</span></span>
<span data-ttu-id="40a23-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="40a23-123">Here is a JSON representation of the resource.</span></span>
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



