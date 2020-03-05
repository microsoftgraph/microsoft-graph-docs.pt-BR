---
title: tipo de recurso osVersionCount
description: Contagem de dispositivos com malware para cada versão do sistema operacional
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d4a75ac62e0744b621300fc5474cfefe0823cab8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524953"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="2d676-103">tipo de recurso osVersionCount</span><span class="sxs-lookup"><span data-stu-id="2d676-103">osVersionCount resource type</span></span>

<span data-ttu-id="2d676-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2d676-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d676-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2d676-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d676-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2d676-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d676-107">Contagem de dispositivos com malware para cada versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="2d676-107">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="2d676-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2d676-108">Properties</span></span>
|<span data-ttu-id="2d676-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d676-109">Property</span></span>|<span data-ttu-id="2d676-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d676-110">Type</span></span>|<span data-ttu-id="2d676-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d676-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d676-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="2d676-112">osVersion</span></span>|<span data-ttu-id="2d676-113">String</span><span class="sxs-lookup"><span data-stu-id="2d676-113">String</span></span>|<span data-ttu-id="2d676-114">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="2d676-114">OS version</span></span>|
|<span data-ttu-id="2d676-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="2d676-115">deviceCount</span></span>|<span data-ttu-id="2d676-116">Int32</span><span class="sxs-lookup"><span data-stu-id="2d676-116">Int32</span></span>|<span data-ttu-id="2d676-117">Contagem de dispositivos com malware para a versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="2d676-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="2d676-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="2d676-118">lastUpdateDateTime</span></span>|<span data-ttu-id="2d676-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d676-119">DateTimeOffset</span></span>|<span data-ttu-id="2d676-120">O carimbo de data/hora da última atualização para a contagem de dispositivos em UTC</span><span class="sxs-lookup"><span data-stu-id="2d676-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d676-121">Relações</span><span class="sxs-lookup"><span data-stu-id="2d676-121">Relationships</span></span>
<span data-ttu-id="2d676-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2d676-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d676-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2d676-123">JSON Representation</span></span>
<span data-ttu-id="2d676-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2d676-124">Here is a JSON representation of the resource.</span></span>
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



