---
title: tipo de recurso osVersionCount
description: Contagem de dispositivos com malware para cada versão do sistema operacional
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6408ee1cef68ade4ccb1c8b90f91ca99a5b75bf4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49230895"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="c1011-103">tipo de recurso osVersionCount</span><span class="sxs-lookup"><span data-stu-id="c1011-103">osVersionCount resource type</span></span>

<span data-ttu-id="c1011-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1011-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1011-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c1011-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1011-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c1011-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1011-107">Contagem de dispositivos com malware para cada versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="c1011-107">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="c1011-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c1011-108">Properties</span></span>
|<span data-ttu-id="c1011-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1011-109">Property</span></span>|<span data-ttu-id="c1011-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1011-110">Type</span></span>|<span data-ttu-id="c1011-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1011-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1011-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="c1011-112">osVersion</span></span>|<span data-ttu-id="c1011-113">String</span><span class="sxs-lookup"><span data-stu-id="c1011-113">String</span></span>|<span data-ttu-id="c1011-114">Versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="c1011-114">OS version</span></span>|
|<span data-ttu-id="c1011-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="c1011-115">deviceCount</span></span>|<span data-ttu-id="c1011-116">Int32</span><span class="sxs-lookup"><span data-stu-id="c1011-116">Int32</span></span>|<span data-ttu-id="c1011-117">Contagem de dispositivos com malware para a versão do sistema operacional</span><span class="sxs-lookup"><span data-stu-id="c1011-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="c1011-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="c1011-118">lastUpdateDateTime</span></span>|<span data-ttu-id="c1011-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1011-119">DateTimeOffset</span></span>|<span data-ttu-id="c1011-120">O carimbo de data/hora da última atualização para a contagem de dispositivos em UTC</span><span class="sxs-lookup"><span data-stu-id="c1011-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1011-121">Relações</span><span class="sxs-lookup"><span data-stu-id="c1011-121">Relationships</span></span>
<span data-ttu-id="c1011-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c1011-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1011-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c1011-123">JSON Representation</span></span>
<span data-ttu-id="c1011-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c1011-124">Here is a JSON representation of the resource.</span></span>
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




