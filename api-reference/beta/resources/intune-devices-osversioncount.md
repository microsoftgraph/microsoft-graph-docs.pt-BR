---
title: tipo de recurso osVersionCount
description: Contagem de dispositivos com malware para cada versão do sistema operacional
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a1ea71a04a87972a1f7375af9458d0a25ab04b49
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725432"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="e4ad3-103">tipo de recurso osVersionCount</span><span class="sxs-lookup"><span data-stu-id="e4ad3-103">osVersionCount resource type</span></span>

<span data-ttu-id="e4ad3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4ad3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4ad3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e4ad3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4ad3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4ad3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4ad3-107">Contagem de dispositivos com malware para cada versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="e4ad3-107">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="e4ad3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e4ad3-108">Properties</span></span>
|<span data-ttu-id="e4ad3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e4ad3-109">Property</span></span>|<span data-ttu-id="e4ad3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4ad3-110">Type</span></span>|<span data-ttu-id="e4ad3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4ad3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4ad3-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="e4ad3-112">osVersion</span></span>|<span data-ttu-id="e4ad3-113">String</span><span class="sxs-lookup"><span data-stu-id="e4ad3-113">String</span></span>|<span data-ttu-id="e4ad3-114">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="e4ad3-114">OS version</span></span>|
|<span data-ttu-id="e4ad3-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="e4ad3-115">deviceCount</span></span>|<span data-ttu-id="e4ad3-116">Int32</span><span class="sxs-lookup"><span data-stu-id="e4ad3-116">Int32</span></span>|<span data-ttu-id="e4ad3-117">Contagem de dispositivos com malware para a versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="e4ad3-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="e4ad3-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="e4ad3-118">lastUpdateDateTime</span></span>|<span data-ttu-id="e4ad3-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4ad3-119">DateTimeOffset</span></span>|<span data-ttu-id="e4ad3-120">O carimbo de data/hora da última atualização para a contagem de dispositivos em UTC</span><span class="sxs-lookup"><span data-stu-id="e4ad3-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4ad3-121">Relações</span><span class="sxs-lookup"><span data-stu-id="e4ad3-121">Relationships</span></span>
<span data-ttu-id="e4ad3-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e4ad3-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4ad3-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e4ad3-123">JSON Representation</span></span>
<span data-ttu-id="e4ad3-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e4ad3-124">Here is a JSON representation of the resource.</span></span>
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





