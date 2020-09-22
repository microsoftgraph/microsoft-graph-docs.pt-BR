---
title: tipo de recurso osVersionCount
description: Contagem de dispositivos com malware para cada versão do sistema operacional
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2243c5c9897e108701b1729832562b781d63ec51
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081143"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="ca855-103">tipo de recurso osVersionCount</span><span class="sxs-lookup"><span data-stu-id="ca855-103">osVersionCount resource type</span></span>

<span data-ttu-id="ca855-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca855-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca855-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ca855-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca855-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ca855-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca855-107">Contagem de dispositivos com malware para cada versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="ca855-107">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="ca855-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ca855-108">Properties</span></span>
|<span data-ttu-id="ca855-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca855-109">Property</span></span>|<span data-ttu-id="ca855-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca855-110">Type</span></span>|<span data-ttu-id="ca855-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca855-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca855-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="ca855-112">osVersion</span></span>|<span data-ttu-id="ca855-113">String</span><span class="sxs-lookup"><span data-stu-id="ca855-113">String</span></span>|<span data-ttu-id="ca855-114">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="ca855-114">OS version</span></span>|
|<span data-ttu-id="ca855-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="ca855-115">deviceCount</span></span>|<span data-ttu-id="ca855-116">Int32</span><span class="sxs-lookup"><span data-stu-id="ca855-116">Int32</span></span>|<span data-ttu-id="ca855-117">Contagem de dispositivos com malware para a versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="ca855-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="ca855-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="ca855-118">lastUpdateDateTime</span></span>|<span data-ttu-id="ca855-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca855-119">DateTimeOffset</span></span>|<span data-ttu-id="ca855-120">O carimbo de data/hora da última atualização para a contagem de dispositivos em UTC</span><span class="sxs-lookup"><span data-stu-id="ca855-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca855-121">Relações</span><span class="sxs-lookup"><span data-stu-id="ca855-121">Relationships</span></span>
<span data-ttu-id="ca855-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ca855-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca855-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ca855-123">JSON Representation</span></span>
<span data-ttu-id="ca855-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ca855-124">Here is a JSON representation of the resource.</span></span>
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






