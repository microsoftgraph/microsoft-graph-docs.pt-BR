---
title: tipo de recurso androidManagedStoreAppTrack
description: Contém informações de acompanhamento de aplicativos de repositório gerenciados do Android.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d505a11016ae9959ff783e15b83d912346365183
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449783"
---
# <a name="androidmanagedstoreapptrack-resource-type"></a><span data-ttu-id="da488-103">tipo de recurso androidManagedStoreAppTrack</span><span class="sxs-lookup"><span data-stu-id="da488-103">androidManagedStoreAppTrack resource type</span></span>

<span data-ttu-id="da488-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da488-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="da488-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="da488-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da488-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="da488-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da488-107">Contém informações de acompanhamento de aplicativos de repositório gerenciados do Android.</span><span class="sxs-lookup"><span data-stu-id="da488-107">Contains track information for Android Managed Store apps.</span></span>

## <a name="properties"></a><span data-ttu-id="da488-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da488-108">Properties</span></span>
|<span data-ttu-id="da488-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da488-109">Property</span></span>|<span data-ttu-id="da488-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="da488-110">Type</span></span>|<span data-ttu-id="da488-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="da488-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da488-112">TrackID</span><span class="sxs-lookup"><span data-stu-id="da488-112">trackId</span></span>|<span data-ttu-id="da488-113">String</span><span class="sxs-lookup"><span data-stu-id="da488-113">String</span></span>|<span data-ttu-id="da488-114">Identificador de faixa exclusivo.</span><span class="sxs-lookup"><span data-stu-id="da488-114">Unique track identifier.</span></span>|
|<span data-ttu-id="da488-115">trackAlias</span><span class="sxs-lookup"><span data-stu-id="da488-115">trackAlias</span></span>|<span data-ttu-id="da488-116">String</span><span class="sxs-lookup"><span data-stu-id="da488-116">String</span></span>|<span data-ttu-id="da488-117">Nome amigável da faixa.</span><span class="sxs-lookup"><span data-stu-id="da488-117">Friendly name for track.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da488-118">Relações</span><span class="sxs-lookup"><span data-stu-id="da488-118">Relationships</span></span>
<span data-ttu-id="da488-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="da488-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da488-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da488-120">JSON Representation</span></span>
<span data-ttu-id="da488-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="da488-121">Here is a JSON representation of the resource.</span></span>
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



