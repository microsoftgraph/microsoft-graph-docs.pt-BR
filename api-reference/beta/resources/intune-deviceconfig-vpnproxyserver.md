---
title: tipo de recurso vpnProxyServer
description: Servidor proxy VPN.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6cf550e25c1f777e9f78fd20bdf2863e79f491b2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43412028"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="d5960-103">tipo de recurso vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="d5960-103">vpnProxyServer resource type</span></span>

<span data-ttu-id="d5960-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5960-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5960-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d5960-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5960-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d5960-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5960-107">Servidor proxy VPN.</span><span class="sxs-lookup"><span data-stu-id="d5960-107">VPN Proxy Server.</span></span>

## <a name="properties"></a><span data-ttu-id="d5960-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5960-108">Properties</span></span>
|<span data-ttu-id="d5960-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5960-109">Property</span></span>|<span data-ttu-id="d5960-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5960-110">Type</span></span>|<span data-ttu-id="d5960-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5960-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5960-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="d5960-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="d5960-113">String</span><span class="sxs-lookup"><span data-stu-id="d5960-113">String</span></span>|<span data-ttu-id="d5960-114">URL do script de configuração automática do proxy.</span><span class="sxs-lookup"><span data-stu-id="d5960-114">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="d5960-115">address</span><span class="sxs-lookup"><span data-stu-id="d5960-115">address</span></span>|<span data-ttu-id="d5960-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5960-116">String</span></span>|<span data-ttu-id="d5960-117">Enfrentar.</span><span class="sxs-lookup"><span data-stu-id="d5960-117">Address.</span></span>|
|<span data-ttu-id="d5960-118">propor</span><span class="sxs-lookup"><span data-stu-id="d5960-118">port</span></span>|<span data-ttu-id="d5960-119">Int32</span><span class="sxs-lookup"><span data-stu-id="d5960-119">Int32</span></span>|<span data-ttu-id="d5960-120">Propor.</span><span class="sxs-lookup"><span data-stu-id="d5960-120">Port.</span></span> <span data-ttu-id="d5960-121">Valores válidos de 0 a 65535</span><span class="sxs-lookup"><span data-stu-id="d5960-121">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5960-122">Relações</span><span class="sxs-lookup"><span data-stu-id="d5960-122">Relationships</span></span>
<span data-ttu-id="d5960-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d5960-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5960-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5960-124">JSON Representation</span></span>
<span data-ttu-id="d5960-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5960-125">Here is a JSON representation of the resource.</span></span>
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



