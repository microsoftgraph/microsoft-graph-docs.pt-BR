---
title: tipo de recurso vpnProxyServer
description: Servidor proxy VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 73b004eaae0b49c9f3e4341c32923d7f2d48ae45
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944576"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="1846b-103">tipo de recurso vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="1846b-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="1846b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1846b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1846b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1846b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1846b-106">Servidor proxy VPN.</span><span class="sxs-lookup"><span data-stu-id="1846b-106">VPN Proxy Server.</span></span>

## <a name="properties"></a><span data-ttu-id="1846b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1846b-107">Properties</span></span>
|<span data-ttu-id="1846b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1846b-108">Property</span></span>|<span data-ttu-id="1846b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1846b-109">Type</span></span>|<span data-ttu-id="1846b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1846b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1846b-111">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="1846b-111">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="1846b-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1846b-112">String</span></span>|<span data-ttu-id="1846b-113">URL do script de configuração automática do proxy.</span><span class="sxs-lookup"><span data-stu-id="1846b-113">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="1846b-114">address</span><span class="sxs-lookup"><span data-stu-id="1846b-114">address</span></span>|<span data-ttu-id="1846b-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1846b-115">String</span></span>|<span data-ttu-id="1846b-116">Enfrentar.</span><span class="sxs-lookup"><span data-stu-id="1846b-116">Address.</span></span>|
|<span data-ttu-id="1846b-117">propor</span><span class="sxs-lookup"><span data-stu-id="1846b-117">port</span></span>|<span data-ttu-id="1846b-118">Int32</span><span class="sxs-lookup"><span data-stu-id="1846b-118">Int32</span></span>|<span data-ttu-id="1846b-119">Propor.</span><span class="sxs-lookup"><span data-stu-id="1846b-119">Port.</span></span> <span data-ttu-id="1846b-120">Valores válidos de 0 a 65535</span><span class="sxs-lookup"><span data-stu-id="1846b-120">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="1846b-121">Relações</span><span class="sxs-lookup"><span data-stu-id="1846b-121">Relationships</span></span>
<span data-ttu-id="1846b-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1846b-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1846b-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1846b-123">JSON Representation</span></span>
<span data-ttu-id="1846b-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1846b-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024
}
```




