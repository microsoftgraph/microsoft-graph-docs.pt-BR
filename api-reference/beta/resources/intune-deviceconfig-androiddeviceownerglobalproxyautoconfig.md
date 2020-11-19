---
title: tipo de recurso androidDeviceOwnerGlobalProxyAutoConfig
description: Configuração automática de proxy global de proprietário do dispositivo Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 70b2fc59c2136364af0f2023b17c9f888fad8b6d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49303535"
---
# <a name="androiddeviceownerglobalproxyautoconfig-resource-type"></a><span data-ttu-id="64aae-103">tipo de recurso androidDeviceOwnerGlobalProxyAutoConfig</span><span class="sxs-lookup"><span data-stu-id="64aae-103">androidDeviceOwnerGlobalProxyAutoConfig resource type</span></span>

<span data-ttu-id="64aae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64aae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64aae-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="64aae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64aae-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="64aae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64aae-107">Configuração automática de proxy global de proprietário do dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="64aae-107">Android Device Owner Global Proxy Auto Config.</span></span>


<span data-ttu-id="64aae-108">Herda de [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="64aae-108">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="64aae-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="64aae-109">Properties</span></span>
|<span data-ttu-id="64aae-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64aae-110">Property</span></span>|<span data-ttu-id="64aae-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="64aae-111">Type</span></span>|<span data-ttu-id="64aae-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="64aae-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64aae-113">proxyAutoConfigURL</span><span class="sxs-lookup"><span data-stu-id="64aae-113">proxyAutoConfigURL</span></span>|<span data-ttu-id="64aae-114">String</span><span class="sxs-lookup"><span data-stu-id="64aae-114">String</span></span>|<span data-ttu-id="64aae-115">A URL de configuração automática do proxy</span><span class="sxs-lookup"><span data-stu-id="64aae-115">The proxy auto-config URL</span></span>|

## <a name="relationships"></a><span data-ttu-id="64aae-116">Relações</span><span class="sxs-lookup"><span data-stu-id="64aae-116">Relationships</span></span>
<span data-ttu-id="64aae-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="64aae-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="64aae-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="64aae-118">JSON Representation</span></span>
<span data-ttu-id="64aae-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="64aae-119">Here is a JSON representation of the resource.</span></span>
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




