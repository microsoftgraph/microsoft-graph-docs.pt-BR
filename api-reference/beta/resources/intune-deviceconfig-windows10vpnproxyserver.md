---
title: tipo de recurso de windows10VpnProxyServer
description: Servidor de Proxy VPN.
ms.openlocfilehash: cae448924087cba4b039eab92c83c8bffc94f9fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036330"
---
# <a name="windows10vpnproxyserver-resource-type"></a><span data-ttu-id="3f5be-103">tipo de recurso de windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="3f5be-103">windows10VpnProxyServer resource type</span></span>

> <span data-ttu-id="3f5be-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3f5be-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3f5be-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3f5be-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3f5be-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3f5be-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3f5be-107">Servidor de Proxy VPN.</span><span class="sxs-lookup"><span data-stu-id="3f5be-107">VPN Proxy Server.</span></span>

<span data-ttu-id="3f5be-108">Herda de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="3f5be-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3f5be-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3f5be-109">Properties</span></span>
|<span data-ttu-id="3f5be-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f5be-110">Property</span></span>|<span data-ttu-id="3f5be-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f5be-111">Type</span></span>|<span data-ttu-id="3f5be-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f5be-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f5be-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="3f5be-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="3f5be-114">String</span><span class="sxs-lookup"><span data-stu-id="3f5be-114">String</span></span>|<span data-ttu-id="3f5be-115">Url de script de configuração automática do proxy.</span><span class="sxs-lookup"><span data-stu-id="3f5be-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="3f5be-116">Herdado de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="3f5be-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="3f5be-117">address</span><span class="sxs-lookup"><span data-stu-id="3f5be-117">address</span></span>|<span data-ttu-id="3f5be-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f5be-118">String</span></span>|<span data-ttu-id="3f5be-119">Endereço.</span><span class="sxs-lookup"><span data-stu-id="3f5be-119">Address.</span></span> <span data-ttu-id="3f5be-120">Herdado de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="3f5be-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="3f5be-121">porta</span><span class="sxs-lookup"><span data-stu-id="3f5be-121">port</span></span>|<span data-ttu-id="3f5be-122">Int32</span><span class="sxs-lookup"><span data-stu-id="3f5be-122">Int32</span></span>|<span data-ttu-id="3f5be-123">Porta.</span><span class="sxs-lookup"><span data-stu-id="3f5be-123">Port.</span></span> <span data-ttu-id="3f5be-124">0 a 65.535 Inherited de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md) de valores válido</span><span class="sxs-lookup"><span data-stu-id="3f5be-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="3f5be-125">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="3f5be-125">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="3f5be-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="3f5be-126">Boolean</span></span>|<span data-ttu-id="3f5be-127">Ignorar servidor proxy para endereços locais.</span><span class="sxs-lookup"><span data-stu-id="3f5be-127">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f5be-128">Relações</span><span class="sxs-lookup"><span data-stu-id="3f5be-128">Relationships</span></span>
<span data-ttu-id="3f5be-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3f5be-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3f5be-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3f5be-130">JSON Representation</span></span>
<span data-ttu-id="3f5be-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3f5be-131">Here is a JSON representation of the resource.</span></span>
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





