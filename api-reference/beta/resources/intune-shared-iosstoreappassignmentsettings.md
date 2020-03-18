---
title: Tipo de recurso iosStoreAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS Store para um grupo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 23cb5d484aaa813bfb1b3cd352cd0168e750713e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42769672"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="5dc2a-103">Tipo de recurso iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="5dc2a-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="5dc2a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5dc2a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5dc2a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5dc2a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5dc2a-106">Contém propriedades usadas para atribuir um aplicativo móvel da iOS Store para um grupo.</span><span class="sxs-lookup"><span data-stu-id="5dc2a-106">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="5dc2a-107">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="5dc2a-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5dc2a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5dc2a-108">Properties</span></span>
|<span data-ttu-id="5dc2a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5dc2a-109">Property</span></span>|<span data-ttu-id="5dc2a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5dc2a-110">Type</span></span>|<span data-ttu-id="5dc2a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dc2a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dc2a-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="5dc2a-112">vpnConfigurationId</span></span>|<span data-ttu-id="5dc2a-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5dc2a-113">String</span></span>|<span data-ttu-id="5dc2a-114">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5dc2a-114">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="5dc2a-115">**Apps**</span><span class="sxs-lookup"><span data-stu-id="5dc2a-115">**Apps**</span></span>|
|<span data-ttu-id="5dc2a-116">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="5dc2a-116">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="5dc2a-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="5dc2a-117">Boolean</span></span>|<span data-ttu-id="5dc2a-118">Se o aplicativo será ou não desinstalado quando o dispositivo for removido do Intune.</span><span class="sxs-lookup"><span data-stu-id="5dc2a-118">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5dc2a-119">Relações</span><span class="sxs-lookup"><span data-stu-id="5dc2a-119">Relationships</span></span>
<span data-ttu-id="5dc2a-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5dc2a-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5dc2a-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5dc2a-121">JSON Representation</span></span>
<span data-ttu-id="5dc2a-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5dc2a-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosStoreAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosStoreAppAssignmentSettings",
  "vpnConfigurationId": "String",
  "uninstallOnDeviceRemoval": true
}
```



