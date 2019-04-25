---
title: tipo de recurso osVersionCount
description: Contagem de dispositivos com malware para cada versão do sistema operacional
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7df4f920335c579e2e17cdeb275cc0545887f1d4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578726"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="f7303-103">tipo de recurso osVersionCount</span><span class="sxs-lookup"><span data-stu-id="f7303-103">osVersionCount resource type</span></span>

> <span data-ttu-id="f7303-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f7303-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7303-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f7303-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7303-106">Contagem de dispositivos com malware para cada versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="f7303-106">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="f7303-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f7303-107">Properties</span></span>
|<span data-ttu-id="f7303-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7303-108">Property</span></span>|<span data-ttu-id="f7303-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7303-109">Type</span></span>|<span data-ttu-id="f7303-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7303-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7303-111">osVersion</span><span class="sxs-lookup"><span data-stu-id="f7303-111">osVersion</span></span>|<span data-ttu-id="f7303-112">String</span><span class="sxs-lookup"><span data-stu-id="f7303-112">String</span></span>|<span data-ttu-id="f7303-113">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="f7303-113">OS version</span></span>|
|<span data-ttu-id="f7303-114">deviceCount</span><span class="sxs-lookup"><span data-stu-id="f7303-114">deviceCount</span></span>|<span data-ttu-id="f7303-115">Int32</span><span class="sxs-lookup"><span data-stu-id="f7303-115">Int32</span></span>|<span data-ttu-id="f7303-116">Contagem de dispositivos com malware para a versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="f7303-116">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="f7303-117">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f7303-117">lastUpdateDateTime</span></span>|<span data-ttu-id="f7303-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7303-118">DateTimeOffset</span></span>|<span data-ttu-id="f7303-119">O carimbo de data/hora da última atualização para a contagem de dispositivos em UTC</span><span class="sxs-lookup"><span data-stu-id="f7303-119">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7303-120">Relações</span><span class="sxs-lookup"><span data-stu-id="f7303-120">Relationships</span></span>
<span data-ttu-id="f7303-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f7303-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7303-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f7303-122">JSON Representation</span></span>
<span data-ttu-id="f7303-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f7303-123">Here is a JSON representation of the resource.</span></span>
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





