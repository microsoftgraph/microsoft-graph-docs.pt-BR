---
title: tipo de recurso osVersionCount
description: Contagem de dispositivos com malware para cada versão do sistema operacional
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d4b8987017012d4db0756fc3d8a78efe99319d68
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963909"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="749f7-103">tipo de recurso osVersionCount</span><span class="sxs-lookup"><span data-stu-id="749f7-103">osVersionCount resource type</span></span>

> <span data-ttu-id="749f7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="749f7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="749f7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="749f7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="749f7-106">Contagem de dispositivos com malware para cada versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="749f7-106">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="749f7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="749f7-107">Properties</span></span>
|<span data-ttu-id="749f7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="749f7-108">Property</span></span>|<span data-ttu-id="749f7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="749f7-109">Type</span></span>|<span data-ttu-id="749f7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="749f7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="749f7-111">osVersion</span><span class="sxs-lookup"><span data-stu-id="749f7-111">osVersion</span></span>|<span data-ttu-id="749f7-112">String</span><span class="sxs-lookup"><span data-stu-id="749f7-112">String</span></span>|<span data-ttu-id="749f7-113">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="749f7-113">OS version</span></span>|
|<span data-ttu-id="749f7-114">deviceCount</span><span class="sxs-lookup"><span data-stu-id="749f7-114">deviceCount</span></span>|<span data-ttu-id="749f7-115">Int32</span><span class="sxs-lookup"><span data-stu-id="749f7-115">Int32</span></span>|<span data-ttu-id="749f7-116">Contagem de dispositivos com malware para a versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="749f7-116">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="749f7-117">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="749f7-117">lastUpdateDateTime</span></span>|<span data-ttu-id="749f7-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="749f7-118">DateTimeOffset</span></span>|<span data-ttu-id="749f7-119">O carimbo de data/hora da última atualização para a contagem de dispositivos em UTC</span><span class="sxs-lookup"><span data-stu-id="749f7-119">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="749f7-120">Relações</span><span class="sxs-lookup"><span data-stu-id="749f7-120">Relationships</span></span>
<span data-ttu-id="749f7-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="749f7-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="749f7-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="749f7-122">JSON Representation</span></span>
<span data-ttu-id="749f7-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="749f7-123">Here is a JSON representation of the resource.</span></span>
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





