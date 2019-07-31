---
title: tipo de recurso vpnProxyServer
description: Servidor proxy VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d9aa15cd1ccf7e299be97d52073924258efd069d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969447"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="9f88a-103">tipo de recurso vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="9f88a-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="9f88a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9f88a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f88a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9f88a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f88a-106">Servidor proxy VPN.</span><span class="sxs-lookup"><span data-stu-id="9f88a-106">VPN Proxy Server.</span></span>

## <a name="properties"></a><span data-ttu-id="9f88a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9f88a-107">Properties</span></span>
|<span data-ttu-id="9f88a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9f88a-108">Property</span></span>|<span data-ttu-id="9f88a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f88a-109">Type</span></span>|<span data-ttu-id="9f88a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f88a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f88a-111">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="9f88a-111">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="9f88a-112">String</span><span class="sxs-lookup"><span data-stu-id="9f88a-112">String</span></span>|<span data-ttu-id="9f88a-113">URL do script de configuração automática do proxy.</span><span class="sxs-lookup"><span data-stu-id="9f88a-113">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="9f88a-114">address</span><span class="sxs-lookup"><span data-stu-id="9f88a-114">address</span></span>|<span data-ttu-id="9f88a-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9f88a-115">String</span></span>|<span data-ttu-id="9f88a-116">Enfrentar.</span><span class="sxs-lookup"><span data-stu-id="9f88a-116">Address.</span></span>|
|<span data-ttu-id="9f88a-117">propor</span><span class="sxs-lookup"><span data-stu-id="9f88a-117">port</span></span>|<span data-ttu-id="9f88a-118">Int32</span><span class="sxs-lookup"><span data-stu-id="9f88a-118">Int32</span></span>|<span data-ttu-id="9f88a-119">Propor.</span><span class="sxs-lookup"><span data-stu-id="9f88a-119">Port.</span></span> <span data-ttu-id="9f88a-120">Valores válidos de 0 a 65535</span><span class="sxs-lookup"><span data-stu-id="9f88a-120">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f88a-121">Relações</span><span class="sxs-lookup"><span data-stu-id="9f88a-121">Relationships</span></span>
<span data-ttu-id="9f88a-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9f88a-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f88a-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9f88a-123">JSON Representation</span></span>
<span data-ttu-id="9f88a-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9f88a-124">Here is a JSON representation of the resource.</span></span>
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





