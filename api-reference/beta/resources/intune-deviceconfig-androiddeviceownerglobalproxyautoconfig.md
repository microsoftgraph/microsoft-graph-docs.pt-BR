---
title: tipo de recurso androidDeviceOwnerGlobalProxyAutoConfig
description: Configuração automática de proxy global de proprietário do dispositivo Android.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6c3acf7ef749a95cd17009284d587e4dd41ef4ec
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797011"
---
# <a name="androiddeviceownerglobalproxyautoconfig-resource-type"></a><span data-ttu-id="e474a-103">tipo de recurso androidDeviceOwnerGlobalProxyAutoConfig</span><span class="sxs-lookup"><span data-stu-id="e474a-103">androidDeviceOwnerGlobalProxyAutoConfig resource type</span></span>

> <span data-ttu-id="e474a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e474a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e474a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e474a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e474a-106">Configuração automática de proxy global de proprietário do dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="e474a-106">Android Device Owner Global Proxy Auto Config.</span></span>


<span data-ttu-id="e474a-107">Herda de [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="e474a-107">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e474a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e474a-108">Properties</span></span>
|<span data-ttu-id="e474a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e474a-109">Property</span></span>|<span data-ttu-id="e474a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e474a-110">Type</span></span>|<span data-ttu-id="e474a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e474a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e474a-112">proxyAutoConfigURL</span><span class="sxs-lookup"><span data-stu-id="e474a-112">proxyAutoConfigURL</span></span>|<span data-ttu-id="e474a-113">String</span><span class="sxs-lookup"><span data-stu-id="e474a-113">String</span></span>|<span data-ttu-id="e474a-114">A URL de configuração automática do proxy</span><span class="sxs-lookup"><span data-stu-id="e474a-114">The proxy auto-config URL</span></span>|

## <a name="relationships"></a><span data-ttu-id="e474a-115">Relações</span><span class="sxs-lookup"><span data-stu-id="e474a-115">Relationships</span></span>
<span data-ttu-id="e474a-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e474a-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e474a-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e474a-117">JSON Representation</span></span>
<span data-ttu-id="e474a-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e474a-118">Here is a JSON representation of the resource.</span></span>
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



