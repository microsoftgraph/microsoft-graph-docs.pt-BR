---
title: tipo de recurso windows81VpnProxyServer
description: Servidor proxy VPN.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 345856eb5032026cd92c33cad07a620e3659f473
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786562"
---
# <a name="windows81vpnproxyserver-resource-type"></a><span data-ttu-id="418c2-103">tipo de recurso windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="418c2-103">windows81VpnProxyServer resource type</span></span>

> <span data-ttu-id="418c2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="418c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="418c2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="418c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="418c2-106">Servidor proxy VPN.</span><span class="sxs-lookup"><span data-stu-id="418c2-106">VPN Proxy Server.</span></span>


<span data-ttu-id="418c2-107">Herda de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="418c2-107">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="418c2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="418c2-108">Properties</span></span>
|<span data-ttu-id="418c2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="418c2-109">Property</span></span>|<span data-ttu-id="418c2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="418c2-110">Type</span></span>|<span data-ttu-id="418c2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="418c2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="418c2-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="418c2-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="418c2-113">String</span><span class="sxs-lookup"><span data-stu-id="418c2-113">String</span></span>|<span data-ttu-id="418c2-114">URL do script de configuração automática do proxy.</span><span class="sxs-lookup"><span data-stu-id="418c2-114">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="418c2-115">Herdado de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="418c2-115">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="418c2-116">address</span><span class="sxs-lookup"><span data-stu-id="418c2-116">address</span></span>|<span data-ttu-id="418c2-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="418c2-117">String</span></span>|<span data-ttu-id="418c2-118">Enfrentar.</span><span class="sxs-lookup"><span data-stu-id="418c2-118">Address.</span></span> <span data-ttu-id="418c2-119">Herdado de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="418c2-119">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="418c2-120">propor</span><span class="sxs-lookup"><span data-stu-id="418c2-120">port</span></span>|<span data-ttu-id="418c2-121">Int32</span><span class="sxs-lookup"><span data-stu-id="418c2-121">Int32</span></span>|<span data-ttu-id="418c2-122">Propor.</span><span class="sxs-lookup"><span data-stu-id="418c2-122">Port.</span></span> <span data-ttu-id="418c2-123">Valores válidos de 0 a 65535 herdados de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="418c2-123">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="418c2-124">automaticallyDetectProxySettings</span><span class="sxs-lookup"><span data-stu-id="418c2-124">automaticallyDetectProxySettings</span></span>|<span data-ttu-id="418c2-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="418c2-125">Boolean</span></span>|<span data-ttu-id="418c2-126">Detectar automaticamente as configurações de proxy.</span><span class="sxs-lookup"><span data-stu-id="418c2-126">Automatically detect proxy settings.</span></span>|
|<span data-ttu-id="418c2-127">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="418c2-127">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="418c2-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="418c2-128">Boolean</span></span>|<span data-ttu-id="418c2-129">Ignorar servidor proxy para endereço local.</span><span class="sxs-lookup"><span data-stu-id="418c2-129">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="418c2-130">Relações</span><span class="sxs-lookup"><span data-stu-id="418c2-130">Relationships</span></span>
<span data-ttu-id="418c2-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="418c2-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="418c2-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="418c2-132">JSON Representation</span></span>
<span data-ttu-id="418c2-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="418c2-133">Here is a JSON representation of the resource.</span></span>
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



