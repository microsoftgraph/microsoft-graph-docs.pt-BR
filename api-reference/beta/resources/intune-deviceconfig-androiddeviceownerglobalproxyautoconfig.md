---
title: tipo de recurso androidDeviceOwnerGlobalProxyAutoConfig
description: Configuração automática de proxy global de proprietário do dispositivo Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 86b00ccbe30568879a58bc1018d9c12fd36fa014
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708918"
---
# <a name="androiddeviceownerglobalproxyautoconfig-resource-type"></a><span data-ttu-id="91b73-103">tipo de recurso androidDeviceOwnerGlobalProxyAutoConfig</span><span class="sxs-lookup"><span data-stu-id="91b73-103">androidDeviceOwnerGlobalProxyAutoConfig resource type</span></span>

<span data-ttu-id="91b73-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91b73-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91b73-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="91b73-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91b73-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="91b73-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91b73-107">Configuração automática de proxy global de proprietário do dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="91b73-107">Android Device Owner Global Proxy Auto Config.</span></span>


<span data-ttu-id="91b73-108">Herda de [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="91b73-108">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="91b73-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="91b73-109">Properties</span></span>
|<span data-ttu-id="91b73-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91b73-110">Property</span></span>|<span data-ttu-id="91b73-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="91b73-111">Type</span></span>|<span data-ttu-id="91b73-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="91b73-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91b73-113">proxyAutoConfigURL</span><span class="sxs-lookup"><span data-stu-id="91b73-113">proxyAutoConfigURL</span></span>|<span data-ttu-id="91b73-114">String</span><span class="sxs-lookup"><span data-stu-id="91b73-114">String</span></span>|<span data-ttu-id="91b73-115">A URL de configuração automática do proxy</span><span class="sxs-lookup"><span data-stu-id="91b73-115">The proxy auto-config URL</span></span>|

## <a name="relationships"></a><span data-ttu-id="91b73-116">Relações</span><span class="sxs-lookup"><span data-stu-id="91b73-116">Relationships</span></span>
<span data-ttu-id="91b73-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="91b73-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91b73-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="91b73-118">JSON Representation</span></span>
<span data-ttu-id="91b73-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="91b73-119">Here is a JSON representation of the resource.</span></span>
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





