---
title: tipo de recurso androidManagedStoreAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel de repositório gerenciado do Android a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 040530a9f14499b964f47c6bd3f2456521b5f742
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259120"
---
# <a name="androidmanagedstoreappassignmentsettings-resource-type"></a><span data-ttu-id="806dc-103">tipo de recurso androidManagedStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="806dc-103">androidManagedStoreAppAssignmentSettings resource type</span></span>

<span data-ttu-id="806dc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="806dc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="806dc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="806dc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="806dc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="806dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="806dc-107">Contém propriedades usadas para atribuir um aplicativo móvel de repositório gerenciado do Android a um grupo.</span><span class="sxs-lookup"><span data-stu-id="806dc-107">Contains properties used to assign an Android Managed Store mobile app to a group.</span></span>


<span data-ttu-id="806dc-108">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="806dc-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="806dc-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="806dc-109">Properties</span></span>
|<span data-ttu-id="806dc-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="806dc-110">Property</span></span>|<span data-ttu-id="806dc-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="806dc-111">Type</span></span>|<span data-ttu-id="806dc-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="806dc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="806dc-113">androidManagedStoreAppTrackIds</span><span class="sxs-lookup"><span data-stu-id="806dc-113">androidManagedStoreAppTrackIds</span></span>|<span data-ttu-id="806dc-114">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="806dc-114">String collection</span></span>|<span data-ttu-id="806dc-115">As IDs de acompanhamento a serem habilitadas para esta atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="806dc-115">The track IDs to enable for this app assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="806dc-116">Relações</span><span class="sxs-lookup"><span data-stu-id="806dc-116">Relationships</span></span>
<span data-ttu-id="806dc-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="806dc-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="806dc-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="806dc-118">JSON Representation</span></span>
<span data-ttu-id="806dc-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="806dc-119">Here is a JSON representation of the resource.</span></span>
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




