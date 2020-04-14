---
title: tipo de recurso androidManagedStoreAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel de repositório gerenciado do Android a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cfdca91e3499a495ba810b1c791653d62c769e4a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440500"
---
# <a name="androidmanagedstoreappassignmentsettings-resource-type"></a><span data-ttu-id="b5c88-103">tipo de recurso androidManagedStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="b5c88-103">androidManagedStoreAppAssignmentSettings resource type</span></span>

<span data-ttu-id="b5c88-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5c88-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5c88-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b5c88-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5c88-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b5c88-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5c88-107">Contém propriedades usadas para atribuir um aplicativo móvel de repositório gerenciado do Android a um grupo.</span><span class="sxs-lookup"><span data-stu-id="b5c88-107">Contains properties used to assign an Android Managed Store mobile app to a group.</span></span>


<span data-ttu-id="b5c88-108">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="b5c88-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b5c88-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b5c88-109">Properties</span></span>
|<span data-ttu-id="b5c88-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b5c88-110">Property</span></span>|<span data-ttu-id="b5c88-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b5c88-111">Type</span></span>|<span data-ttu-id="b5c88-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b5c88-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5c88-113">androidManagedStoreAppTrackIds</span><span class="sxs-lookup"><span data-stu-id="b5c88-113">androidManagedStoreAppTrackIds</span></span>|<span data-ttu-id="b5c88-114">Coleção String</span><span class="sxs-lookup"><span data-stu-id="b5c88-114">String collection</span></span>|<span data-ttu-id="b5c88-115">As IDs de acompanhamento a serem habilitadas para esta atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b5c88-115">The track IDs to enable for this app assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5c88-116">Relações</span><span class="sxs-lookup"><span data-stu-id="b5c88-116">Relationships</span></span>
<span data-ttu-id="b5c88-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b5c88-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5c88-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b5c88-118">JSON Representation</span></span>
<span data-ttu-id="b5c88-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b5c88-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppAssignmentSettings",
  "androidManagedStoreAppTrackIds": [
    "String"
  ]
}
```



