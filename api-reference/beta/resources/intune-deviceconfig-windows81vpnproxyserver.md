---
title: tipo de recurso windows81VpnProxyServer
description: Servidor proxy VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 60b8e18be9f50d912020d741cf1d65f1f9d756a4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279147"
---
# <a name="windows81vpnproxyserver-resource-type"></a><span data-ttu-id="e6702-103">tipo de recurso windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="e6702-103">windows81VpnProxyServer resource type</span></span>

<span data-ttu-id="e6702-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6702-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e6702-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e6702-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6702-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e6702-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6702-107">Servidor proxy VPN.</span><span class="sxs-lookup"><span data-stu-id="e6702-107">VPN Proxy Server.</span></span>


<span data-ttu-id="e6702-108">Herda de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="e6702-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e6702-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6702-109">Properties</span></span>
|<span data-ttu-id="e6702-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6702-110">Property</span></span>|<span data-ttu-id="e6702-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6702-111">Type</span></span>|<span data-ttu-id="e6702-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6702-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6702-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="e6702-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="e6702-114">String</span><span class="sxs-lookup"><span data-stu-id="e6702-114">String</span></span>|<span data-ttu-id="e6702-115">URL do script de configuração automática do proxy.</span><span class="sxs-lookup"><span data-stu-id="e6702-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="e6702-116">Herdado de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="e6702-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="e6702-117">address</span><span class="sxs-lookup"><span data-stu-id="e6702-117">address</span></span>|<span data-ttu-id="e6702-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6702-118">String</span></span>|<span data-ttu-id="e6702-119">Enfrentar.</span><span class="sxs-lookup"><span data-stu-id="e6702-119">Address.</span></span> <span data-ttu-id="e6702-120">Herdado de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="e6702-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="e6702-121">propor</span><span class="sxs-lookup"><span data-stu-id="e6702-121">port</span></span>|<span data-ttu-id="e6702-122">Int32</span><span class="sxs-lookup"><span data-stu-id="e6702-122">Int32</span></span>|<span data-ttu-id="e6702-123">Propor.</span><span class="sxs-lookup"><span data-stu-id="e6702-123">Port.</span></span> <span data-ttu-id="e6702-124">Valores válidos de 0 a 65535 herdados de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="e6702-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="e6702-125">automaticallyDetectProxySettings</span><span class="sxs-lookup"><span data-stu-id="e6702-125">automaticallyDetectProxySettings</span></span>|<span data-ttu-id="e6702-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="e6702-126">Boolean</span></span>|<span data-ttu-id="e6702-127">Detectar automaticamente as configurações de proxy.</span><span class="sxs-lookup"><span data-stu-id="e6702-127">Automatically detect proxy settings.</span></span>|
|<span data-ttu-id="e6702-128">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="e6702-128">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="e6702-129">Booliano</span><span class="sxs-lookup"><span data-stu-id="e6702-129">Boolean</span></span>|<span data-ttu-id="e6702-130">Ignorar servidor proxy para endereço local.</span><span class="sxs-lookup"><span data-stu-id="e6702-130">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6702-131">Relações</span><span class="sxs-lookup"><span data-stu-id="e6702-131">Relationships</span></span>
<span data-ttu-id="e6702-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6702-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6702-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6702-133">JSON Representation</span></span>
<span data-ttu-id="e6702-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e6702-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows81VpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81VpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024,
  "automaticallyDetectProxySettings": true,
  "bypassProxyServerForLocalAddress": true
}
```




