---
title: tipo de recurso de windows81VpnProxyServer
description: Servidor de Proxy VPN.
author: tfitzmac
ms.openlocfilehash: 015df762d25e1a87a9ce29bd4efbc15e98ed7e08
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349361"
---
# <a name="windows81vpnproxyserver-resource-type"></a><span data-ttu-id="c1406-103">tipo de recurso de windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="c1406-103">windows81VpnProxyServer resource type</span></span>

> <span data-ttu-id="c1406-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c1406-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1406-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c1406-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1406-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c1406-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c1406-107">Servidor de Proxy VPN.</span><span class="sxs-lookup"><span data-stu-id="c1406-107">VPN Proxy Server.</span></span>

<span data-ttu-id="c1406-108">Herda de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="c1406-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c1406-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c1406-109">Properties</span></span>
|<span data-ttu-id="c1406-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1406-110">Property</span></span>|<span data-ttu-id="c1406-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1406-111">Type</span></span>|<span data-ttu-id="c1406-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1406-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1406-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="c1406-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="c1406-114">String</span><span class="sxs-lookup"><span data-stu-id="c1406-114">String</span></span>|<span data-ttu-id="c1406-115">Url de script de configuração automática do proxy.</span><span class="sxs-lookup"><span data-stu-id="c1406-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="c1406-116">Herdado de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="c1406-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="c1406-117">address</span><span class="sxs-lookup"><span data-stu-id="c1406-117">address</span></span>|<span data-ttu-id="c1406-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1406-118">String</span></span>|<span data-ttu-id="c1406-119">Endereço.</span><span class="sxs-lookup"><span data-stu-id="c1406-119">Address.</span></span> <span data-ttu-id="c1406-120">Herdado de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="c1406-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="c1406-121">porta</span><span class="sxs-lookup"><span data-stu-id="c1406-121">port</span></span>|<span data-ttu-id="c1406-122">Int32</span><span class="sxs-lookup"><span data-stu-id="c1406-122">Int32</span></span>|<span data-ttu-id="c1406-123">Porta.</span><span class="sxs-lookup"><span data-stu-id="c1406-123">Port.</span></span> <span data-ttu-id="c1406-124">0 a 65.535 Inherited de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md) de valores válido</span><span class="sxs-lookup"><span data-stu-id="c1406-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="c1406-125">automaticallyDetectProxySettings</span><span class="sxs-lookup"><span data-stu-id="c1406-125">automaticallyDetectProxySettings</span></span>|<span data-ttu-id="c1406-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1406-126">Boolean</span></span>|<span data-ttu-id="c1406-127">Detecte automaticamente as configurações de proxy.</span><span class="sxs-lookup"><span data-stu-id="c1406-127">Automatically detect proxy settings.</span></span>|
|<span data-ttu-id="c1406-128">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="c1406-128">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="c1406-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1406-129">Boolean</span></span>|<span data-ttu-id="c1406-130">Ignorar servidor proxy para endereços locais.</span><span class="sxs-lookup"><span data-stu-id="c1406-130">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1406-131">Relações</span><span class="sxs-lookup"><span data-stu-id="c1406-131">Relationships</span></span>
<span data-ttu-id="c1406-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c1406-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c1406-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c1406-133">JSON Representation</span></span>
<span data-ttu-id="c1406-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c1406-134">Here is a JSON representation of the resource.</span></span>
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





