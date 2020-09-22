---
title: tipo de recurso androidDeviceOwnerGlobalProxyDirect
description: Proxy global do proprietário do dispositivo Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 020ad601a261427df8a573c38e4b992a830d31bc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085154"
---
# <a name="androiddeviceownerglobalproxydirect-resource-type"></a><span data-ttu-id="bbc59-103">tipo de recurso androidDeviceOwnerGlobalProxyDirect</span><span class="sxs-lookup"><span data-stu-id="bbc59-103">androidDeviceOwnerGlobalProxyDirect resource type</span></span>

<span data-ttu-id="bbc59-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbc59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bbc59-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bbc59-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbc59-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bbc59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbc59-107">Proxy global do proprietário do dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="bbc59-107">Android Device Owner Global Proxy Direct.</span></span>


<span data-ttu-id="bbc59-108">Herda de [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="bbc59-108">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bbc59-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bbc59-109">Properties</span></span>
|<span data-ttu-id="bbc59-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bbc59-110">Property</span></span>|<span data-ttu-id="bbc59-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbc59-111">Type</span></span>|<span data-ttu-id="bbc59-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbc59-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbc59-113">host</span><span class="sxs-lookup"><span data-stu-id="bbc59-113">host</span></span>|<span data-ttu-id="bbc59-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bbc59-114">String</span></span>|<span data-ttu-id="bbc59-115">O nome do host</span><span class="sxs-lookup"><span data-stu-id="bbc59-115">The host name</span></span>|
|<span data-ttu-id="bbc59-116">propor</span><span class="sxs-lookup"><span data-stu-id="bbc59-116">port</span></span>|<span data-ttu-id="bbc59-117">Int32</span><span class="sxs-lookup"><span data-stu-id="bbc59-117">Int32</span></span>|<span data-ttu-id="bbc59-118">A porta</span><span class="sxs-lookup"><span data-stu-id="bbc59-118">The port</span></span>|
|<span data-ttu-id="bbc59-119">excludedHosts</span><span class="sxs-lookup"><span data-stu-id="bbc59-119">excludedHosts</span></span>|<span data-ttu-id="bbc59-120">Coleção String</span><span class="sxs-lookup"><span data-stu-id="bbc59-120">String collection</span></span>|<span data-ttu-id="bbc59-121">Os hosts excluídos</span><span class="sxs-lookup"><span data-stu-id="bbc59-121">The excluded hosts</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbc59-122">Relações</span><span class="sxs-lookup"><span data-stu-id="bbc59-122">Relationships</span></span>
<span data-ttu-id="bbc59-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bbc59-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bbc59-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bbc59-124">JSON Representation</span></span>
<span data-ttu-id="bbc59-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bbc59-125">Here is a JSON representation of the resource.</span></span>
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






