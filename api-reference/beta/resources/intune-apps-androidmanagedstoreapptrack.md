---
title: tipo de recurso androidManagedStoreAppTrack
description: Contém informações de acompanhamento de aplicativos de repositório gerenciados do Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ab4009dfb8fc6cfd40ae49529e07a6a6932d7c4d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690270"
---
# <a name="androidmanagedstoreapptrack-resource-type"></a><span data-ttu-id="8630d-103">tipo de recurso androidManagedStoreAppTrack</span><span class="sxs-lookup"><span data-stu-id="8630d-103">androidManagedStoreAppTrack resource type</span></span>

<span data-ttu-id="8630d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8630d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8630d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8630d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8630d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8630d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8630d-107">Contém informações de acompanhamento de aplicativos de repositório gerenciados do Android.</span><span class="sxs-lookup"><span data-stu-id="8630d-107">Contains track information for Android Managed Store apps.</span></span>

## <a name="properties"></a><span data-ttu-id="8630d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8630d-108">Properties</span></span>
|<span data-ttu-id="8630d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8630d-109">Property</span></span>|<span data-ttu-id="8630d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8630d-110">Type</span></span>|<span data-ttu-id="8630d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8630d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8630d-112">TrackID</span><span class="sxs-lookup"><span data-stu-id="8630d-112">trackId</span></span>|<span data-ttu-id="8630d-113">String</span><span class="sxs-lookup"><span data-stu-id="8630d-113">String</span></span>|<span data-ttu-id="8630d-114">Identificador de faixa exclusivo.</span><span class="sxs-lookup"><span data-stu-id="8630d-114">Unique track identifier.</span></span>|
|<span data-ttu-id="8630d-115">trackAlias</span><span class="sxs-lookup"><span data-stu-id="8630d-115">trackAlias</span></span>|<span data-ttu-id="8630d-116">String</span><span class="sxs-lookup"><span data-stu-id="8630d-116">String</span></span>|<span data-ttu-id="8630d-117">Nome amigável da faixa.</span><span class="sxs-lookup"><span data-stu-id="8630d-117">Friendly name for track.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8630d-118">Relações</span><span class="sxs-lookup"><span data-stu-id="8630d-118">Relationships</span></span>
<span data-ttu-id="8630d-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8630d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8630d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8630d-120">JSON Representation</span></span>
<span data-ttu-id="8630d-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8630d-121">Here is a JSON representation of the resource.</span></span>
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





