---
title: Tipo de recurso iosVppAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 987f020bbdae683a1ff8df9439af698c2102918b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523650"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="34450-103">Tipo de recurso iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="34450-103">iosVppAppAssignmentSettings resource type</span></span>

<span data-ttu-id="34450-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="34450-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34450-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="34450-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34450-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="34450-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34450-107">Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="34450-107">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="34450-108">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="34450-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="34450-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34450-109">Properties</span></span>
|<span data-ttu-id="34450-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34450-110">Property</span></span>|<span data-ttu-id="34450-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="34450-111">Type</span></span>|<span data-ttu-id="34450-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="34450-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34450-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="34450-113">useDeviceLicensing</span></span>|<span data-ttu-id="34450-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="34450-114">Boolean</span></span>|<span data-ttu-id="34450-115">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="34450-115">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="34450-116">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="34450-116">vpnConfigurationId</span></span>|<span data-ttu-id="34450-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34450-117">String</span></span>|<span data-ttu-id="34450-118">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="34450-118">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="34450-119">**Apps**</span><span class="sxs-lookup"><span data-stu-id="34450-119">**Apps**</span></span>|
|<span data-ttu-id="34450-120">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="34450-120">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="34450-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="34450-121">Boolean</span></span>|<span data-ttu-id="34450-122">Se o aplicativo será ou não desinstalado quando o dispositivo for removido do Intune.</span><span class="sxs-lookup"><span data-stu-id="34450-122">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34450-123">Relações</span><span class="sxs-lookup"><span data-stu-id="34450-123">Relationships</span></span>
<span data-ttu-id="34450-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="34450-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34450-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="34450-125">JSON Representation</span></span>
<span data-ttu-id="34450-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="34450-126">Here is a JSON representation of the resource.</span></span>
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



