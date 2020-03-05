---
title: tipo de recurso androidDeviceOwnerGlobalProxyAutoConfig
description: Configuração automática de proxy global de proprietário do dispositivo Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 207cbafb423b322fd954d561a4204150cb078abf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42486595"
---
# <a name="androiddeviceownerglobalproxyautoconfig-resource-type"></a><span data-ttu-id="6ae78-103">tipo de recurso androidDeviceOwnerGlobalProxyAutoConfig</span><span class="sxs-lookup"><span data-stu-id="6ae78-103">androidDeviceOwnerGlobalProxyAutoConfig resource type</span></span>

<span data-ttu-id="6ae78-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6ae78-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ae78-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6ae78-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ae78-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6ae78-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ae78-107">Configuração automática de proxy global de proprietário do dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="6ae78-107">Android Device Owner Global Proxy Auto Config.</span></span>


<span data-ttu-id="6ae78-108">Herda de [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="6ae78-108">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6ae78-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6ae78-109">Properties</span></span>
|<span data-ttu-id="6ae78-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6ae78-110">Property</span></span>|<span data-ttu-id="6ae78-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ae78-111">Type</span></span>|<span data-ttu-id="6ae78-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ae78-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ae78-113">proxyAutoConfigURL</span><span class="sxs-lookup"><span data-stu-id="6ae78-113">proxyAutoConfigURL</span></span>|<span data-ttu-id="6ae78-114">String</span><span class="sxs-lookup"><span data-stu-id="6ae78-114">String</span></span>|<span data-ttu-id="6ae78-115">A URL de configuração automática do proxy</span><span class="sxs-lookup"><span data-stu-id="6ae78-115">The proxy auto-config URL</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ae78-116">Relações</span><span class="sxs-lookup"><span data-stu-id="6ae78-116">Relationships</span></span>
<span data-ttu-id="6ae78-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6ae78-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ae78-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6ae78-118">JSON Representation</span></span>
<span data-ttu-id="6ae78-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6ae78-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
  "proxyAutoConfigURL": "String"
}
```



