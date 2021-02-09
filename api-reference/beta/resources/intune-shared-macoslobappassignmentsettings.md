---
title: Tipo de recurso macOsLobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo LOB do Mac a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3e00019e2ed7609aa02fc3f16b2076027617fcab
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160299"
---
# <a name="macoslobappassignmentsettings-resource-type"></a><span data-ttu-id="62f57-103">Tipo de recurso macOsLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="62f57-103">macOsLobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="62f57-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62f57-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="62f57-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="62f57-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62f57-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="62f57-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62f57-107">Contém propriedades usadas para atribuir um aplicativo LOB do Mac a um grupo.</span><span class="sxs-lookup"><span data-stu-id="62f57-107">Contains properties used to assign an Mac LOB  app to a group.</span></span>


<span data-ttu-id="62f57-108">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="62f57-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="62f57-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62f57-109">Properties</span></span>
|<span data-ttu-id="62f57-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62f57-110">Property</span></span>|<span data-ttu-id="62f57-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="62f57-111">Type</span></span>|<span data-ttu-id="62f57-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="62f57-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62f57-113">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="62f57-113">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="62f57-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="62f57-114">Boolean</span></span>|<span data-ttu-id="62f57-115">Se o aplicativo será ou não desinstalado quando o dispositivo for removido do Intune.</span><span class="sxs-lookup"><span data-stu-id="62f57-115">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62f57-116">Relações</span><span class="sxs-lookup"><span data-stu-id="62f57-116">Relationships</span></span>
<span data-ttu-id="62f57-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="62f57-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="62f57-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="62f57-118">JSON Representation</span></span>
<span data-ttu-id="62f57-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="62f57-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsLobAppAssignmentSettings",
  "uninstallOnDeviceRemoval": true
}
```




