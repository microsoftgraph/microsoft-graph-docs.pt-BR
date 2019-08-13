---
title: Tipo de recurso iosVppAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bb4fd7e4a2cded97bdd5d61921cd1819908a4d77
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366774"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="40e1f-103">Tipo de recurso iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="40e1f-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="40e1f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="40e1f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40e1f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="40e1f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40e1f-106">Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="40e1f-106">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="40e1f-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="40e1f-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="40e1f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="40e1f-108">Properties</span></span>
|<span data-ttu-id="40e1f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40e1f-109">Property</span></span>|<span data-ttu-id="40e1f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="40e1f-110">Type</span></span>|<span data-ttu-id="40e1f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="40e1f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40e1f-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="40e1f-112">useDeviceLicensing</span></span>|<span data-ttu-id="40e1f-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e1f-113">Boolean</span></span>|<span data-ttu-id="40e1f-114">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="40e1f-114">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="40e1f-115">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="40e1f-115">vpnConfigurationId</span></span>|<span data-ttu-id="40e1f-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40e1f-116">String</span></span>|<span data-ttu-id="40e1f-117">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="40e1f-117">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="40e1f-118">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="40e1f-118">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="40e1f-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="40e1f-119">Boolean</span></span>|<span data-ttu-id="40e1f-120">Se o aplicativo será ou não desinstalado quando o dispositivo for removido do Intune.</span><span class="sxs-lookup"><span data-stu-id="40e1f-120">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40e1f-121">Relações</span><span class="sxs-lookup"><span data-stu-id="40e1f-121">Relationships</span></span>
<span data-ttu-id="40e1f-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="40e1f-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="40e1f-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="40e1f-123">JSON Representation</span></span>
<span data-ttu-id="40e1f-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="40e1f-124">Here is a JSON representation of the resource.</span></span>
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



