---
title: tipo de recurso windows10VpnProxyServer
description: Servidor proxy VPN.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d68a21863febb3339fe4fcd218d87418428bafe9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43317885"
---
# <a name="windows10vpnproxyserver-resource-type"></a><span data-ttu-id="0c669-103">tipo de recurso windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="0c669-103">windows10VpnProxyServer resource type</span></span>

<span data-ttu-id="0c669-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c669-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c669-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0c669-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c669-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0c669-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c669-107">Servidor proxy VPN.</span><span class="sxs-lookup"><span data-stu-id="0c669-107">VPN Proxy Server.</span></span>


<span data-ttu-id="0c669-108">Herda de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="0c669-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0c669-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c669-109">Properties</span></span>
|<span data-ttu-id="0c669-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c669-110">Property</span></span>|<span data-ttu-id="0c669-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c669-111">Type</span></span>|<span data-ttu-id="0c669-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c669-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c669-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="0c669-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="0c669-114">String</span><span class="sxs-lookup"><span data-stu-id="0c669-114">String</span></span>|<span data-ttu-id="0c669-115">URL do script de configuração automática do proxy.</span><span class="sxs-lookup"><span data-stu-id="0c669-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="0c669-116">Herdado de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="0c669-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="0c669-117">address</span><span class="sxs-lookup"><span data-stu-id="0c669-117">address</span></span>|<span data-ttu-id="0c669-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c669-118">String</span></span>|<span data-ttu-id="0c669-119">Enfrentar.</span><span class="sxs-lookup"><span data-stu-id="0c669-119">Address.</span></span> <span data-ttu-id="0c669-120">Herdado de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="0c669-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="0c669-121">propor</span><span class="sxs-lookup"><span data-stu-id="0c669-121">port</span></span>|<span data-ttu-id="0c669-122">Int32</span><span class="sxs-lookup"><span data-stu-id="0c669-122">Int32</span></span>|<span data-ttu-id="0c669-123">Propor.</span><span class="sxs-lookup"><span data-stu-id="0c669-123">Port.</span></span> <span data-ttu-id="0c669-124">Valores válidos de 0 a 65535 herdados de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="0c669-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="0c669-125">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="0c669-125">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="0c669-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="0c669-126">Boolean</span></span>|<span data-ttu-id="0c669-127">Ignorar servidor proxy para endereço local.</span><span class="sxs-lookup"><span data-stu-id="0c669-127">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c669-128">Relações</span><span class="sxs-lookup"><span data-stu-id="0c669-128">Relationships</span></span>
<span data-ttu-id="0c669-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0c669-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c669-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c669-130">JSON Representation</span></span>
<span data-ttu-id="0c669-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0c669-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10VpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10VpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024,
  "bypassProxyServerForLocalAddress": true
}
```



