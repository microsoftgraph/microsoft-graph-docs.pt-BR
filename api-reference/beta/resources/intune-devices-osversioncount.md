---
title: tipo de recurso osVersionCount
description: Contagem de dispositivos com malware para cada versão do sistema operacional
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4654f49d6d58d07dbb349edf38d4336da82a4aeb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783918"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="1abd9-103">tipo de recurso osVersionCount</span><span class="sxs-lookup"><span data-stu-id="1abd9-103">osVersionCount resource type</span></span>

> <span data-ttu-id="1abd9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1abd9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1abd9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1abd9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1abd9-106">Contagem de dispositivos com malware para cada versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="1abd9-106">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="1abd9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1abd9-107">Properties</span></span>
|<span data-ttu-id="1abd9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1abd9-108">Property</span></span>|<span data-ttu-id="1abd9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1abd9-109">Type</span></span>|<span data-ttu-id="1abd9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1abd9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1abd9-111">osVersion</span><span class="sxs-lookup"><span data-stu-id="1abd9-111">osVersion</span></span>|<span data-ttu-id="1abd9-112">String</span><span class="sxs-lookup"><span data-stu-id="1abd9-112">String</span></span>|<span data-ttu-id="1abd9-113">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="1abd9-113">OS version</span></span>|
|<span data-ttu-id="1abd9-114">deviceCount</span><span class="sxs-lookup"><span data-stu-id="1abd9-114">deviceCount</span></span>|<span data-ttu-id="1abd9-115">Int32</span><span class="sxs-lookup"><span data-stu-id="1abd9-115">Int32</span></span>|<span data-ttu-id="1abd9-116">Contagem de dispositivos com malware para a versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="1abd9-116">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="1abd9-117">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="1abd9-117">lastUpdateDateTime</span></span>|<span data-ttu-id="1abd9-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1abd9-118">DateTimeOffset</span></span>|<span data-ttu-id="1abd9-119">O carimbo de data/hora da última atualização para a contagem de dispositivos em UTC</span><span class="sxs-lookup"><span data-stu-id="1abd9-119">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="1abd9-120">Relações</span><span class="sxs-lookup"><span data-stu-id="1abd9-120">Relationships</span></span>
<span data-ttu-id="1abd9-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1abd9-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1abd9-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1abd9-122">JSON Representation</span></span>
<span data-ttu-id="1abd9-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1abd9-123">Here is a JSON representation of the resource.</span></span>
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



