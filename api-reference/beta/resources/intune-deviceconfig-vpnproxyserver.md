---
title: tipo de recurso vpnProxyServer
description: Servidor proxy VPN.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b8a452cdde7c4c360107a67396d8f5ce49d6eb1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145273"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="75c0c-103">tipo de recurso vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="75c0c-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="75c0c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="75c0c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75c0c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75c0c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75c0c-106">Servidor proxy VPN.</span><span class="sxs-lookup"><span data-stu-id="75c0c-106">VPN Proxy Server.</span></span>

## <a name="properties"></a><span data-ttu-id="75c0c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="75c0c-107">Properties</span></span>
|<span data-ttu-id="75c0c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75c0c-108">Property</span></span>|<span data-ttu-id="75c0c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="75c0c-109">Type</span></span>|<span data-ttu-id="75c0c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="75c0c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75c0c-111">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="75c0c-111">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="75c0c-112">String</span><span class="sxs-lookup"><span data-stu-id="75c0c-112">String</span></span>|<span data-ttu-id="75c0c-113">URL do script de configuração automática do proxy.</span><span class="sxs-lookup"><span data-stu-id="75c0c-113">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="75c0c-114">address</span><span class="sxs-lookup"><span data-stu-id="75c0c-114">address</span></span>|<span data-ttu-id="75c0c-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="75c0c-115">String</span></span>|<span data-ttu-id="75c0c-116">Enfrentar.</span><span class="sxs-lookup"><span data-stu-id="75c0c-116">Address.</span></span>|
|<span data-ttu-id="75c0c-117">porta</span><span class="sxs-lookup"><span data-stu-id="75c0c-117">port</span></span>|<span data-ttu-id="75c0c-118">Int32</span><span class="sxs-lookup"><span data-stu-id="75c0c-118">Int32</span></span>|<span data-ttu-id="75c0c-119">Propor.</span><span class="sxs-lookup"><span data-stu-id="75c0c-119">Port.</span></span> <span data-ttu-id="75c0c-120">Valores válidos de 0 a 65535</span><span class="sxs-lookup"><span data-stu-id="75c0c-120">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="75c0c-121">Relações</span><span class="sxs-lookup"><span data-stu-id="75c0c-121">Relationships</span></span>
<span data-ttu-id="75c0c-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="75c0c-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="75c0c-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75c0c-123">JSON Representation</span></span>
<span data-ttu-id="75c0c-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="75c0c-124">Here is a JSON representation of the resource.</span></span>
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




