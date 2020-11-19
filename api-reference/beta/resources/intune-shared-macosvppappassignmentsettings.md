---
title: tipo de recurso macOsVppAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel do Mac VPP a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fbd6d9193bc9a441caf66662dab42bcb7648d374
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49258945"
---
# <a name="macosvppappassignmentsettings-resource-type"></a><span data-ttu-id="09913-103">tipo de recurso macOsVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="09913-103">macOsVppAppAssignmentSettings resource type</span></span>

<span data-ttu-id="09913-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09913-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09913-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="09913-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09913-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="09913-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09913-107">Contém propriedades usadas para atribuir um aplicativo móvel do Mac VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="09913-107">Contains properties used to assign an Mac VPP mobile app to a group.</span></span>


<span data-ttu-id="09913-108">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="09913-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="09913-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="09913-109">Properties</span></span>
|<span data-ttu-id="09913-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09913-110">Property</span></span>|<span data-ttu-id="09913-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="09913-111">Type</span></span>|<span data-ttu-id="09913-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="09913-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09913-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="09913-113">useDeviceLicensing</span></span>|<span data-ttu-id="09913-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="09913-114">Boolean</span></span>|<span data-ttu-id="09913-115">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="09913-115">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="09913-116">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="09913-116">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="09913-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="09913-117">Boolean</span></span>|<span data-ttu-id="09913-118">Se o aplicativo será ou não desinstalado quando o dispositivo for removido do Intune.</span><span class="sxs-lookup"><span data-stu-id="09913-118">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09913-119">Relações</span><span class="sxs-lookup"><span data-stu-id="09913-119">Relationships</span></span>
<span data-ttu-id="09913-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="09913-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09913-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="09913-121">JSON Representation</span></span>
<span data-ttu-id="09913-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="09913-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignmentSettings",
  "useDeviceLicensing": true,
  "uninstallOnDeviceRemoval": true
}
```




