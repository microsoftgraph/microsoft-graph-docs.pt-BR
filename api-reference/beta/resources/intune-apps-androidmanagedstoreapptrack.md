---
title: tipo de recurso androidManagedStoreAppTrack
description: Contém informações de acompanhamento de aplicativos de repositório gerenciados do Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0444165a3dfb86efa1f4fc25e2edf0ea309b6959
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004071"
---
# <a name="androidmanagedstoreapptrack-resource-type"></a><span data-ttu-id="35d4f-103">tipo de recurso androidManagedStoreAppTrack</span><span class="sxs-lookup"><span data-stu-id="35d4f-103">androidManagedStoreAppTrack resource type</span></span>

<span data-ttu-id="35d4f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35d4f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="35d4f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="35d4f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35d4f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="35d4f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35d4f-107">Contém informações de acompanhamento de aplicativos de repositório gerenciados do Android.</span><span class="sxs-lookup"><span data-stu-id="35d4f-107">Contains track information for Android Managed Store apps.</span></span>

## <a name="properties"></a><span data-ttu-id="35d4f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="35d4f-108">Properties</span></span>
|<span data-ttu-id="35d4f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35d4f-109">Property</span></span>|<span data-ttu-id="35d4f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="35d4f-110">Type</span></span>|<span data-ttu-id="35d4f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="35d4f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35d4f-112">TrackID</span><span class="sxs-lookup"><span data-stu-id="35d4f-112">trackId</span></span>|<span data-ttu-id="35d4f-113">String</span><span class="sxs-lookup"><span data-stu-id="35d4f-113">String</span></span>|<span data-ttu-id="35d4f-114">Identificador de faixa exclusivo.</span><span class="sxs-lookup"><span data-stu-id="35d4f-114">Unique track identifier.</span></span>|
|<span data-ttu-id="35d4f-115">trackAlias</span><span class="sxs-lookup"><span data-stu-id="35d4f-115">trackAlias</span></span>|<span data-ttu-id="35d4f-116">String</span><span class="sxs-lookup"><span data-stu-id="35d4f-116">String</span></span>|<span data-ttu-id="35d4f-117">Nome amigável da faixa.</span><span class="sxs-lookup"><span data-stu-id="35d4f-117">Friendly name for track.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35d4f-118">Relações</span><span class="sxs-lookup"><span data-stu-id="35d4f-118">Relationships</span></span>
<span data-ttu-id="35d4f-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="35d4f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35d4f-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="35d4f-120">JSON Representation</span></span>
<span data-ttu-id="35d4f-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="35d4f-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppTrack"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppTrack",
  "trackId": "String",
  "trackAlias": "String"
}
```






