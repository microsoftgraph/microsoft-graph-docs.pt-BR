---
title: tipo de recurso de windows10VpnProxyServer
description: Servidor de Proxy VPN.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d4f8975a08e60105c37e0959ac72e24a1dd639cd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407120"
---
# <a name="windows10vpnproxyserver-resource-type"></a><span data-ttu-id="97483-103">tipo de recurso de windows10VpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="97483-103">windows10VpnProxyServer resource type</span></span>

> <span data-ttu-id="97483-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="97483-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="97483-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="97483-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="97483-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="97483-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97483-107">Servidor de Proxy VPN.</span><span class="sxs-lookup"><span data-stu-id="97483-107">VPN Proxy Server.</span></span>


<span data-ttu-id="97483-108">Herda de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="97483-108">Inherits from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>

## <a name="properties"></a><span data-ttu-id="97483-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="97483-109">Properties</span></span>
|<span data-ttu-id="97483-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97483-110">Property</span></span>|<span data-ttu-id="97483-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="97483-111">Type</span></span>|<span data-ttu-id="97483-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="97483-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97483-113">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="97483-113">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="97483-114">String</span><span class="sxs-lookup"><span data-stu-id="97483-114">String</span></span>|<span data-ttu-id="97483-115">Url de script de configuração automática do proxy.</span><span class="sxs-lookup"><span data-stu-id="97483-115">Proxy's automatic configuration script url.</span></span> <span data-ttu-id="97483-116">Herdado de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="97483-116">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="97483-117">address</span><span class="sxs-lookup"><span data-stu-id="97483-117">address</span></span>|<span data-ttu-id="97483-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="97483-118">String</span></span>|<span data-ttu-id="97483-119">Endereço.</span><span class="sxs-lookup"><span data-stu-id="97483-119">Address.</span></span> <span data-ttu-id="97483-120">Herdado de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span><span class="sxs-lookup"><span data-stu-id="97483-120">Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="97483-121">porta</span><span class="sxs-lookup"><span data-stu-id="97483-121">port</span></span>|<span data-ttu-id="97483-122">Int32</span><span class="sxs-lookup"><span data-stu-id="97483-122">Int32</span></span>|<span data-ttu-id="97483-123">Porta.</span><span class="sxs-lookup"><span data-stu-id="97483-123">Port.</span></span> <span data-ttu-id="97483-124">0 a 65.535 Inherited de [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md) de valores válido</span><span class="sxs-lookup"><span data-stu-id="97483-124">Valid values 0 to 65535 Inherited from [vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)</span></span>|
|<span data-ttu-id="97483-125">bypassProxyServerForLocalAddress</span><span class="sxs-lookup"><span data-stu-id="97483-125">bypassProxyServerForLocalAddress</span></span>|<span data-ttu-id="97483-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="97483-126">Boolean</span></span>|<span data-ttu-id="97483-127">Ignorar servidor proxy para endereços locais.</span><span class="sxs-lookup"><span data-stu-id="97483-127">Bypass proxy server for local address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97483-128">Relações</span><span class="sxs-lookup"><span data-stu-id="97483-128">Relationships</span></span>
<span data-ttu-id="97483-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="97483-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97483-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="97483-130">JSON Representation</span></span>
<span data-ttu-id="97483-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="97483-131">Here is a JSON representation of the resource.</span></span>
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




