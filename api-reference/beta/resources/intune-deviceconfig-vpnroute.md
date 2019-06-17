---
title: tipo de recurso vpnRoute
description: Definição da rota VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 89b07a6f58bcd8ce5159c5bec07d01d2beea9fdd
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987534"
---
# <a name="vpnroute-resource-type"></a><span data-ttu-id="349ff-103">tipo de recurso vpnRoute</span><span class="sxs-lookup"><span data-stu-id="349ff-103">vpnRoute resource type</span></span>

> <span data-ttu-id="349ff-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="349ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="349ff-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="349ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="349ff-106">Definição da rota VPN.</span><span class="sxs-lookup"><span data-stu-id="349ff-106">VPN Route definition.</span></span>

## <a name="properties"></a><span data-ttu-id="349ff-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="349ff-107">Properties</span></span>
|<span data-ttu-id="349ff-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="349ff-108">Property</span></span>|<span data-ttu-id="349ff-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="349ff-109">Type</span></span>|<span data-ttu-id="349ff-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="349ff-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="349ff-111">destinationPrefix</span><span class="sxs-lookup"><span data-stu-id="349ff-111">destinationPrefix</span></span>|<span data-ttu-id="349ff-112">String</span><span class="sxs-lookup"><span data-stu-id="349ff-112">String</span></span>|<span data-ttu-id="349ff-113">Prefixo de destino (endereço IPv4/V6).</span><span class="sxs-lookup"><span data-stu-id="349ff-113">Destination prefix (IPv4/v6 address).</span></span>|
|<span data-ttu-id="349ff-114">prefixSize</span><span class="sxs-lookup"><span data-stu-id="349ff-114">prefixSize</span></span>|<span data-ttu-id="349ff-115">Int32</span><span class="sxs-lookup"><span data-stu-id="349ff-115">Int32</span></span>|<span data-ttu-id="349ff-116">Tamanho do prefixo.</span><span class="sxs-lookup"><span data-stu-id="349ff-116">Prefix size.</span></span> <span data-ttu-id="349ff-117">(1-32).</span><span class="sxs-lookup"><span data-stu-id="349ff-117">(1-32).</span></span> <span data-ttu-id="349ff-118">Valores válidos de 1 a 32</span><span class="sxs-lookup"><span data-stu-id="349ff-118">Valid values 1 to 32</span></span>|

## <a name="relationships"></a><span data-ttu-id="349ff-119">Relações</span><span class="sxs-lookup"><span data-stu-id="349ff-119">Relationships</span></span>
<span data-ttu-id="349ff-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="349ff-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="349ff-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="349ff-121">JSON Representation</span></span>
<span data-ttu-id="349ff-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="349ff-122">Here is a JSON representation of the resource.</span></span>
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





