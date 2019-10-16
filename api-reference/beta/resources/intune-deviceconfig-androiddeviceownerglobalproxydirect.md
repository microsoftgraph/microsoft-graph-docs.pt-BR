---
title: tipo de recurso androidDeviceOwnerGlobalProxyDirect
description: Proxy global do proprietário do dispositivo Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cbe4329aacdfb151e0bb5b73f8b24b624010c327
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538641"
---
# <a name="androiddeviceownerglobalproxydirect-resource-type"></a><span data-ttu-id="5a0f5-103">tipo de recurso androidDeviceOwnerGlobalProxyDirect</span><span class="sxs-lookup"><span data-stu-id="5a0f5-103">androidDeviceOwnerGlobalProxyDirect resource type</span></span>

> <span data-ttu-id="5a0f5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5a0f5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5a0f5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5a0f5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a0f5-106">Proxy global do proprietário do dispositivo Android.</span><span class="sxs-lookup"><span data-stu-id="5a0f5-106">Android Device Owner Global Proxy Direct.</span></span>


<span data-ttu-id="5a0f5-107">Herda de [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="5a0f5-107">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5a0f5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5a0f5-108">Properties</span></span>
|<span data-ttu-id="5a0f5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a0f5-109">Property</span></span>|<span data-ttu-id="5a0f5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a0f5-110">Type</span></span>|<span data-ttu-id="5a0f5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a0f5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a0f5-112">host</span><span class="sxs-lookup"><span data-stu-id="5a0f5-112">host</span></span>|<span data-ttu-id="5a0f5-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5a0f5-113">String</span></span>|<span data-ttu-id="5a0f5-114">O nome do host</span><span class="sxs-lookup"><span data-stu-id="5a0f5-114">The host name</span></span>|
|<span data-ttu-id="5a0f5-115">propor</span><span class="sxs-lookup"><span data-stu-id="5a0f5-115">port</span></span>|<span data-ttu-id="5a0f5-116">Int32</span><span class="sxs-lookup"><span data-stu-id="5a0f5-116">Int32</span></span>|<span data-ttu-id="5a0f5-117">A porta</span><span class="sxs-lookup"><span data-stu-id="5a0f5-117">The port</span></span>|
|<span data-ttu-id="5a0f5-118">excludedHosts</span><span class="sxs-lookup"><span data-stu-id="5a0f5-118">excludedHosts</span></span>|<span data-ttu-id="5a0f5-119">String collection</span><span class="sxs-lookup"><span data-stu-id="5a0f5-119">String collection</span></span>|<span data-ttu-id="5a0f5-120">Os hosts excluídos</span><span class="sxs-lookup"><span data-stu-id="5a0f5-120">The excluded hosts</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a0f5-121">Relações</span><span class="sxs-lookup"><span data-stu-id="5a0f5-121">Relationships</span></span>
<span data-ttu-id="5a0f5-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5a0f5-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a0f5-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5a0f5-123">JSON Representation</span></span>
<span data-ttu-id="5a0f5-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5a0f5-124">Here is a JSON representation of the resource.</span></span>
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



