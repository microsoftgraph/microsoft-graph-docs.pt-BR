---
title: tipo de recurso androidDeviceOwnerGlobalProxyAutoConfig
description: Configuração automática de proxy global de proprietário do dispositivo Android.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3cee579dbd5a8dee57b270e117a0c50aca377f94
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43402982"
---
# <a name="androiddeviceownerglobalproxyautoconfig-resource-type"></a><span data-ttu-id="67d17-103">tipo de recurso androidDeviceOwnerGlobalProxyAutoConfig</span><span class="sxs-lookup"><span data-stu-id="67d17-103">androidDeviceOwnerGlobalProxyAutoConfig resource type</span></span>

<span data-ttu-id="67d17-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67d17-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67d17-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="67d17-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67d17-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67d17-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67d17-107">Configuração automática de proxy global de proprietário do dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="67d17-107">Android Device Owner Global Proxy Auto Config.</span></span>


<span data-ttu-id="67d17-108">Herda de [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="67d17-108">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="67d17-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="67d17-109">Properties</span></span>
|<span data-ttu-id="67d17-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67d17-110">Property</span></span>|<span data-ttu-id="67d17-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="67d17-111">Type</span></span>|<span data-ttu-id="67d17-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="67d17-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67d17-113">proxyAutoConfigURL</span><span class="sxs-lookup"><span data-stu-id="67d17-113">proxyAutoConfigURL</span></span>|<span data-ttu-id="67d17-114">String</span><span class="sxs-lookup"><span data-stu-id="67d17-114">String</span></span>|<span data-ttu-id="67d17-115">A URL de configuração automática do proxy</span><span class="sxs-lookup"><span data-stu-id="67d17-115">The proxy auto-config URL</span></span>|

## <a name="relationships"></a><span data-ttu-id="67d17-116">Relações</span><span class="sxs-lookup"><span data-stu-id="67d17-116">Relationships</span></span>
<span data-ttu-id="67d17-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="67d17-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="67d17-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="67d17-118">JSON Representation</span></span>
<span data-ttu-id="67d17-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="67d17-119">Here is a JSON representation of the resource.</span></span>
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



