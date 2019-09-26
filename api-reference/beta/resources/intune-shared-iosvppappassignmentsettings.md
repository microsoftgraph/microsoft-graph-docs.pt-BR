---
title: Tipo de recurso iosVppAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 04e2bedc18d16b1f882835eabdc32b87a9cff5a4
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199599"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="113f9-103">Tipo de recurso iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="113f9-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="113f9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="113f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="113f9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="113f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="113f9-106">Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="113f9-106">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="113f9-107">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="113f9-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="113f9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="113f9-108">Properties</span></span>
|<span data-ttu-id="113f9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="113f9-109">Property</span></span>|<span data-ttu-id="113f9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="113f9-110">Type</span></span>|<span data-ttu-id="113f9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="113f9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="113f9-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="113f9-112">useDeviceLicensing</span></span>|<span data-ttu-id="113f9-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="113f9-113">Boolean</span></span>|<span data-ttu-id="113f9-114">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="113f9-114">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="113f9-115">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="113f9-115">vpnConfigurationId</span></span>|<span data-ttu-id="113f9-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="113f9-116">String</span></span>|<span data-ttu-id="113f9-117">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="113f9-117">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="113f9-118">**Apps**</span><span class="sxs-lookup"><span data-stu-id="113f9-118">**Apps**</span></span>|
|<span data-ttu-id="113f9-119">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="113f9-119">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="113f9-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="113f9-120">Boolean</span></span>|<span data-ttu-id="113f9-121">Se o aplicativo será ou não desinstalado quando o dispositivo for removido do Intune.</span><span class="sxs-lookup"><span data-stu-id="113f9-121">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="113f9-122">Relações</span><span class="sxs-lookup"><span data-stu-id="113f9-122">Relationships</span></span>
<span data-ttu-id="113f9-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="113f9-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="113f9-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="113f9-124">JSON Representation</span></span>
<span data-ttu-id="113f9-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="113f9-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignmentSettings",
  "useDeviceLicensing": true,
  "vpnConfigurationId": "String",
  "uninstallOnDeviceRemoval": true
}
```



