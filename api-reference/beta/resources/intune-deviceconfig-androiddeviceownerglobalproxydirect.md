---
title: tipo de recurso androidDeviceOwnerGlobalProxyDirect
description: Proxy global do proprietário do dispositivo Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 58e95490fa3fd7adaec6e6b8f01c43566b1c289a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42486546"
---
# <a name="androiddeviceownerglobalproxydirect-resource-type"></a><span data-ttu-id="0af01-103">tipo de recurso androidDeviceOwnerGlobalProxyDirect</span><span class="sxs-lookup"><span data-stu-id="0af01-103">androidDeviceOwnerGlobalProxyDirect resource type</span></span>

<span data-ttu-id="0af01-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="0af01-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0af01-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0af01-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0af01-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0af01-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0af01-107">Proxy global do proprietário do dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="0af01-107">Android Device Owner Global Proxy Direct.</span></span>


<span data-ttu-id="0af01-108">Herda de [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="0af01-108">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0af01-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0af01-109">Properties</span></span>
|<span data-ttu-id="0af01-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0af01-110">Property</span></span>|<span data-ttu-id="0af01-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="0af01-111">Type</span></span>|<span data-ttu-id="0af01-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0af01-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0af01-113">host</span><span class="sxs-lookup"><span data-stu-id="0af01-113">host</span></span>|<span data-ttu-id="0af01-114">String</span><span class="sxs-lookup"><span data-stu-id="0af01-114">String</span></span>|<span data-ttu-id="0af01-115">O nome do host</span><span class="sxs-lookup"><span data-stu-id="0af01-115">The host name</span></span>|
|<span data-ttu-id="0af01-116">propor</span><span class="sxs-lookup"><span data-stu-id="0af01-116">port</span></span>|<span data-ttu-id="0af01-117">Int32</span><span class="sxs-lookup"><span data-stu-id="0af01-117">Int32</span></span>|<span data-ttu-id="0af01-118">A porta</span><span class="sxs-lookup"><span data-stu-id="0af01-118">The port</span></span>|
|<span data-ttu-id="0af01-119">excludedHosts</span><span class="sxs-lookup"><span data-stu-id="0af01-119">excludedHosts</span></span>|<span data-ttu-id="0af01-120">String collection</span><span class="sxs-lookup"><span data-stu-id="0af01-120">String collection</span></span>|<span data-ttu-id="0af01-121">Os hosts excluídos</span><span class="sxs-lookup"><span data-stu-id="0af01-121">The excluded hosts</span></span>|

## <a name="relationships"></a><span data-ttu-id="0af01-122">Relações</span><span class="sxs-lookup"><span data-stu-id="0af01-122">Relationships</span></span>
<span data-ttu-id="0af01-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0af01-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0af01-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0af01-124">JSON Representation</span></span>
<span data-ttu-id="0af01-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0af01-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyDirect"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGlobalProxyDirect",
  "host": "String",
  "port": 1024,
  "excludedHosts": [
    "String"
  ]
}
```



