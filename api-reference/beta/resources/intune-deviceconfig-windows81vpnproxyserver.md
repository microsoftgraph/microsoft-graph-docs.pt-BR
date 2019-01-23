---
title: tipo de recurso de windows81VpnProxyServer
description: Servidor de Proxy VPN.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a400ed128a80e6fae11f090f7cdd445fe8c174b0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398888"
---
# <a name="windows81vpnproxyserver-resource-type"></a><span data-ttu-id="4ed6f-103">tipo de recurso de windows81VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="4ed6f-103">windows81VpnProxyServer resource type</span></span>

> <span data-ttu-id="4ed6f-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="4ed6f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4ed6f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4ed6f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4ed6f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="4ed6f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ed6f-107">Servidor de Proxy VPN.</span><span class="sxs-lookup"><span data-stu-id="4ed6f-107">VPN Proxy Server.</span></span>


<span data-ttu-id="4ed6f-108">Herda de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="4ed6f-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4ed6f-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4ed6f-109">Properties</span></span>
|<span data-ttu-id="4ed6f-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ed6f-110">Property</span></span>|<span data-ttu-id="4ed6f-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ed6f-111">Type</span></span>|<span data-ttu-id="4ed6f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ed6f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ed6f-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="4ed6f-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="4ed6f-114">String</span><span class="sxs-lookup"><span data-stu-id="4ed6f-114">String</span></span>|<span data-ttu-id="4ed6f-115">Url de script de configuração automática do proxy.</span><span class="sxs-lookup"><span data-stu-id="4ed6f-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="4ed6f-116">Herdado de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="4ed6f-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="4ed6f-117">address</span><span class="sxs-lookup"><span data-stu-id="4ed6f-117">address</span></span>|<span data-ttu-id="4ed6f-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4ed6f-118">String</span></span>|<span data-ttu-id="4ed6f-119">Endereço.</span><span class="sxs-lookup"><span data-stu-id="4ed6f-119">Address.</span></span> <span data-ttu-id="4ed6f-120">Herdado de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="4ed6f-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="4ed6f-121">porta</span><span class="sxs-lookup"><span data-stu-id="4ed6f-121">port</span></span>|<span data-ttu-id="4ed6f-122">Int32</span><span class="sxs-lookup"><span data-stu-id="4ed6f-122">Int32</span></span>|<span data-ttu-id="4ed6f-123">Porta.</span><span class="sxs-lookup"><span data-stu-id="4ed6f-123">Port.</span></span> <span data-ttu-id="4ed6f-124">0 a 65.535 Inherited de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md) de valores válido</span><span class="sxs-lookup"><span data-stu-id="4ed6f-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="4ed6f-125">automaticallyDetectProxySettings</span><span class="sxs-lookup"><span data-stu-id="4ed6f-125">automaticallyDetectProxySettings</span></span>|<span data-ttu-id="4ed6f-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ed6f-126">Boolean</span></span>|<span data-ttu-id="4ed6f-127">Detecte automaticamente as configurações de proxy.</span><span class="sxs-lookup"><span data-stu-id="4ed6f-127">Automatically detect proxy settings.</span></span>|
|<span data-ttu-id="4ed6f-128">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="4ed6f-128">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="4ed6f-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ed6f-129">Boolean</span></span>|<span data-ttu-id="4ed6f-130">Ignorar servidor proxy para endereços locais.</span><span class="sxs-lookup"><span data-stu-id="4ed6f-130">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ed6f-131">Relações</span><span class="sxs-lookup"><span data-stu-id="4ed6f-131">Relationships</span></span>
<span data-ttu-id="4ed6f-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4ed6f-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ed6f-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ed6f-133">JSON Representation</span></span>
<span data-ttu-id="4ed6f-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4ed6f-134">Here is a JSON representation of the resource.</span></span>
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




