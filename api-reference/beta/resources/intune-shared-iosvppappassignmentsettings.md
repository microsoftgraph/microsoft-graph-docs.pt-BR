---
title: Tipo de recurso iosVppAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5b3f9f3b055cf05460a417098603e8854d11e92f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49300581"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="258b7-103">Tipo de recurso iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="258b7-103">iosVppAppAssignmentSettings resource type</span></span>

<span data-ttu-id="258b7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="258b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="258b7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="258b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="258b7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="258b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="258b7-107">Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="258b7-107">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="258b7-108">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="258b7-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="258b7-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="258b7-109">Properties</span></span>
|<span data-ttu-id="258b7-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="258b7-110">Property</span></span>|<span data-ttu-id="258b7-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="258b7-111">Type</span></span>|<span data-ttu-id="258b7-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="258b7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="258b7-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="258b7-113">useDeviceLicensing</span></span>|<span data-ttu-id="258b7-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="258b7-114">Boolean</span></span>|<span data-ttu-id="258b7-115">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="258b7-115">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="258b7-116">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="258b7-116">vpnConfigurationId</span></span>|<span data-ttu-id="258b7-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="258b7-117">String</span></span>|<span data-ttu-id="258b7-118">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="258b7-118">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="258b7-119">**Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="258b7-119">**Apps**</span></span>|
|<span data-ttu-id="258b7-120">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="258b7-120">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="258b7-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="258b7-121">Boolean</span></span>|<span data-ttu-id="258b7-122">Se o aplicativo será ou não desinstalado quando o dispositivo for removido do Intune.</span><span class="sxs-lookup"><span data-stu-id="258b7-122">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="258b7-123">Relações</span><span class="sxs-lookup"><span data-stu-id="258b7-123">Relationships</span></span>
<span data-ttu-id="258b7-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="258b7-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="258b7-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="258b7-125">JSON Representation</span></span>
<span data-ttu-id="258b7-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="258b7-126">Here is a JSON representation of the resource.</span></span>
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




