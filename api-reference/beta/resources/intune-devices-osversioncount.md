---
title: tipo de recurso osVersionCount
description: Contagem de dispositivos com malware para cada versão do sistema operacional
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12ee68855f45ed6827f84a64084118c24081d266
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142746"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="a21fa-103">tipo de recurso osVersionCount</span><span class="sxs-lookup"><span data-stu-id="a21fa-103">osVersionCount resource type</span></span>

> <span data-ttu-id="a21fa-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a21fa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a21fa-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a21fa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a21fa-106">Contagem de dispositivos com malware para cada versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="a21fa-106">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="a21fa-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a21fa-107">Properties</span></span>
|<span data-ttu-id="a21fa-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a21fa-108">Property</span></span>|<span data-ttu-id="a21fa-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a21fa-109">Type</span></span>|<span data-ttu-id="a21fa-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a21fa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a21fa-111">osVersion</span><span class="sxs-lookup"><span data-stu-id="a21fa-111">osVersion</span></span>|<span data-ttu-id="a21fa-112">String</span><span class="sxs-lookup"><span data-stu-id="a21fa-112">String</span></span>|<span data-ttu-id="a21fa-113">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="a21fa-113">OS version</span></span>|
|<span data-ttu-id="a21fa-114">deviceCount</span><span class="sxs-lookup"><span data-stu-id="a21fa-114">deviceCount</span></span>|<span data-ttu-id="a21fa-115">Int32</span><span class="sxs-lookup"><span data-stu-id="a21fa-115">Int32</span></span>|<span data-ttu-id="a21fa-116">Contagem de dispositivos com malware para a versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="a21fa-116">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="a21fa-117">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="a21fa-117">lastUpdateDateTime</span></span>|<span data-ttu-id="a21fa-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a21fa-118">DateTimeOffset</span></span>|<span data-ttu-id="a21fa-119">O carimbo de data/hora da última atualização para a contagem de dispositivos em UTC</span><span class="sxs-lookup"><span data-stu-id="a21fa-119">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="a21fa-120">Relações</span><span class="sxs-lookup"><span data-stu-id="a21fa-120">Relationships</span></span>
<span data-ttu-id="a21fa-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a21fa-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a21fa-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a21fa-122">JSON Representation</span></span>
<span data-ttu-id="a21fa-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a21fa-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.osVersionCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.osVersionCount",
  "osVersion": "String",
  "deviceCount": 1024,
  "lastUpdateDateTime": "String (timestamp)"
}
```




