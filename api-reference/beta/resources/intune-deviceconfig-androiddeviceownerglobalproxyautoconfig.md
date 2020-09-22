---
title: tipo de recurso androidDeviceOwnerGlobalProxyAutoConfig
description: Configuração automática de proxy global de proprietário do dispositivo Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d6bbc652d3191d7129a0c44546e2360ccabbf0c7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085168"
---
# <a name="androiddeviceownerglobalproxyautoconfig-resource-type"></a><span data-ttu-id="c2500-103">tipo de recurso androidDeviceOwnerGlobalProxyAutoConfig</span><span class="sxs-lookup"><span data-stu-id="c2500-103">androidDeviceOwnerGlobalProxyAutoConfig resource type</span></span>

<span data-ttu-id="c2500-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2500-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2500-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c2500-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2500-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c2500-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2500-107">Configuração automática de proxy global de proprietário do dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="c2500-107">Android Device Owner Global Proxy Auto Config.</span></span>


<span data-ttu-id="c2500-108">Herda de [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="c2500-108">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c2500-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c2500-109">Properties</span></span>
|<span data-ttu-id="c2500-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c2500-110">Property</span></span>|<span data-ttu-id="c2500-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2500-111">Type</span></span>|<span data-ttu-id="c2500-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2500-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2500-113">proxyAutoConfigURL</span><span class="sxs-lookup"><span data-stu-id="c2500-113">proxyAutoConfigURL</span></span>|<span data-ttu-id="c2500-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c2500-114">String</span></span>|<span data-ttu-id="c2500-115">A URL de configuração automática do proxy</span><span class="sxs-lookup"><span data-stu-id="c2500-115">The proxy auto-config URL</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2500-116">Relações</span><span class="sxs-lookup"><span data-stu-id="c2500-116">Relationships</span></span>
<span data-ttu-id="c2500-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c2500-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2500-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c2500-118">JSON Representation</span></span>
<span data-ttu-id="c2500-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c2500-119">Here is a JSON representation of the resource.</span></span>
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






