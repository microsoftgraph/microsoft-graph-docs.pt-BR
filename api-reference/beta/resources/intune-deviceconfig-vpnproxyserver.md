---
title: tipo de recurso vpnProxyServer
description: Servidor proxy VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 013511c027600dd8e787959dc967d99b47c21bc8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728318"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="b177e-103">tipo de recurso vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="b177e-103">vpnProxyServer resource type</span></span>

<span data-ttu-id="b177e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b177e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b177e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b177e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b177e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b177e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b177e-107">Servidor proxy VPN.</span><span class="sxs-lookup"><span data-stu-id="b177e-107">VPN Proxy Server.</span></span>

## <a name="properties"></a><span data-ttu-id="b177e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b177e-108">Properties</span></span>
|<span data-ttu-id="b177e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b177e-109">Property</span></span>|<span data-ttu-id="b177e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b177e-110">Type</span></span>|<span data-ttu-id="b177e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b177e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b177e-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="b177e-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="b177e-113">String</span><span class="sxs-lookup"><span data-stu-id="b177e-113">String</span></span>|<span data-ttu-id="b177e-114">URL do script de configuração automática do proxy.</span><span class="sxs-lookup"><span data-stu-id="b177e-114">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="b177e-115">address</span><span class="sxs-lookup"><span data-stu-id="b177e-115">address</span></span>|<span data-ttu-id="b177e-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b177e-116">String</span></span>|<span data-ttu-id="b177e-117">Enfrentar.</span><span class="sxs-lookup"><span data-stu-id="b177e-117">Address.</span></span>|
|<span data-ttu-id="b177e-118">propor</span><span class="sxs-lookup"><span data-stu-id="b177e-118">port</span></span>|<span data-ttu-id="b177e-119">Int32</span><span class="sxs-lookup"><span data-stu-id="b177e-119">Int32</span></span>|<span data-ttu-id="b177e-120">Propor.</span><span class="sxs-lookup"><span data-stu-id="b177e-120">Port.</span></span> <span data-ttu-id="b177e-121">Valores válidos de 0 a 65535</span><span class="sxs-lookup"><span data-stu-id="b177e-121">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="b177e-122">Relações</span><span class="sxs-lookup"><span data-stu-id="b177e-122">Relationships</span></span>
<span data-ttu-id="b177e-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b177e-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b177e-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b177e-124">JSON Representation</span></span>
<span data-ttu-id="b177e-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b177e-125">Here is a JSON representation of the resource.</span></span>
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





