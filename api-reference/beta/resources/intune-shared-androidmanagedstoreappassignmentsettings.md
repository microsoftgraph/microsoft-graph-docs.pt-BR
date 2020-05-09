---
title: tipo de recurso androidManagedStoreAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel de repositório gerenciado do Android a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cfdca91e3499a495ba810b1c791653d62c769e4a
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178210"
---
# <a name="androidmanagedstoreappassignmentsettings-resource-type"></a><span data-ttu-id="eb23a-103">tipo de recurso androidManagedStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="eb23a-103">androidManagedStoreAppAssignmentSettings resource type</span></span>

<span data-ttu-id="eb23a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb23a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eb23a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eb23a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb23a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eb23a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb23a-107">Contém propriedades usadas para atribuir um aplicativo móvel de repositório gerenciado do Android a um grupo.</span><span class="sxs-lookup"><span data-stu-id="eb23a-107">Contains properties used to assign an Android Managed Store mobile app to a group.</span></span>


<span data-ttu-id="eb23a-108">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="eb23a-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eb23a-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb23a-109">Properties</span></span>
|<span data-ttu-id="eb23a-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb23a-110">Property</span></span>|<span data-ttu-id="eb23a-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb23a-111">Type</span></span>|<span data-ttu-id="eb23a-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb23a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb23a-113">androidManagedStoreAppTrackIds</span><span class="sxs-lookup"><span data-stu-id="eb23a-113">androidManagedStoreAppTrackIds</span></span>|<span data-ttu-id="eb23a-114">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb23a-114">String collection</span></span>|<span data-ttu-id="eb23a-115">As IDs de acompanhamento a serem habilitadas para esta atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="eb23a-115">The track IDs to enable for this app assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb23a-116">Relações</span><span class="sxs-lookup"><span data-stu-id="eb23a-116">Relationships</span></span>
<span data-ttu-id="eb23a-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eb23a-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb23a-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb23a-118">JSON Representation</span></span>
<span data-ttu-id="eb23a-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb23a-119">Here is a JSON representation of the resource.</span></span>
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



