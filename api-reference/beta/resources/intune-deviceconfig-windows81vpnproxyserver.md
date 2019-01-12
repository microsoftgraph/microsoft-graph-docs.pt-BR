---
title: tipo de recurso de windows81VpnProxyServer
description: Servidor de Proxy VPN.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d276ee7ac84bfe86c197025c05bf1a119b85e06c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917956"
---
# <a name="windows81vpnproxyserver-resource-type"></a><span data-ttu-id="16ac8-103">tipo de recurso de windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="16ac8-103">windows81VpnProxyServer resource type</span></span>

> <span data-ttu-id="16ac8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="16ac8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16ac8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="16ac8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16ac8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="16ac8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16ac8-107">Servidor de Proxy VPN.</span><span class="sxs-lookup"><span data-stu-id="16ac8-107">VPN Proxy Server.</span></span>

<span data-ttu-id="16ac8-108">Herda de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="16ac8-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="16ac8-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="16ac8-109">Properties</span></span>
|<span data-ttu-id="16ac8-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16ac8-110">Property</span></span>|<span data-ttu-id="16ac8-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="16ac8-111">Type</span></span>|<span data-ttu-id="16ac8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="16ac8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16ac8-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="16ac8-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="16ac8-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16ac8-114">String</span></span>|<span data-ttu-id="16ac8-115">Url de script de configuração automática do proxy.</span><span class="sxs-lookup"><span data-stu-id="16ac8-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="16ac8-116">Herdado de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="16ac8-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="16ac8-117">address</span><span class="sxs-lookup"><span data-stu-id="16ac8-117">address</span></span>|<span data-ttu-id="16ac8-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16ac8-118">String</span></span>|<span data-ttu-id="16ac8-119">Endereço.</span><span class="sxs-lookup"><span data-stu-id="16ac8-119">Address.</span></span> <span data-ttu-id="16ac8-120">Herdado de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="16ac8-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="16ac8-121">porta</span><span class="sxs-lookup"><span data-stu-id="16ac8-121">port</span></span>|<span data-ttu-id="16ac8-122">Int32</span><span class="sxs-lookup"><span data-stu-id="16ac8-122">Int32</span></span>|<span data-ttu-id="16ac8-123">Porta.</span><span class="sxs-lookup"><span data-stu-id="16ac8-123">Port.</span></span> <span data-ttu-id="16ac8-124">0 a 65.535 Inherited de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md) de valores válido</span><span class="sxs-lookup"><span data-stu-id="16ac8-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="16ac8-125">automaticallyDetectProxySettings</span><span class="sxs-lookup"><span data-stu-id="16ac8-125">automaticallyDetectProxySettings</span></span>|<span data-ttu-id="16ac8-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="16ac8-126">Boolean</span></span>|<span data-ttu-id="16ac8-127">Detecte automaticamente as configurações de proxy.</span><span class="sxs-lookup"><span data-stu-id="16ac8-127">Automatically detect proxy settings.</span></span>|
|<span data-ttu-id="16ac8-128">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="16ac8-128">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="16ac8-129">Booliano</span><span class="sxs-lookup"><span data-stu-id="16ac8-129">Boolean</span></span>|<span data-ttu-id="16ac8-130">Ignorar servidor proxy para endereços locais.</span><span class="sxs-lookup"><span data-stu-id="16ac8-130">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16ac8-131">Relações</span><span class="sxs-lookup"><span data-stu-id="16ac8-131">Relationships</span></span>
<span data-ttu-id="16ac8-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="16ac8-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="16ac8-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="16ac8-133">JSON Representation</span></span>
<span data-ttu-id="16ac8-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="16ac8-134">Here is a JSON representation of the resource.</span></span>
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





