---
title: Tipo de recurso iosVppAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8a72f1876d0d0dcd181aee7a9b0322f372838377
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42769567"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="bf81c-103">Tipo de recurso iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="bf81c-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="bf81c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bf81c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf81c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bf81c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf81c-106">Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="bf81c-106">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="bf81c-107">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="bf81c-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bf81c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bf81c-108">Properties</span></span>
|<span data-ttu-id="bf81c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bf81c-109">Property</span></span>|<span data-ttu-id="bf81c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf81c-110">Type</span></span>|<span data-ttu-id="bf81c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf81c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf81c-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="bf81c-112">useDeviceLicensing</span></span>|<span data-ttu-id="bf81c-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="bf81c-113">Boolean</span></span>|<span data-ttu-id="bf81c-114">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="bf81c-114">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="bf81c-115">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="bf81c-115">vpnConfigurationId</span></span>|<span data-ttu-id="bf81c-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bf81c-116">String</span></span>|<span data-ttu-id="bf81c-117">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bf81c-117">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="bf81c-118">**Apps**</span><span class="sxs-lookup"><span data-stu-id="bf81c-118">**Apps**</span></span>|
|<span data-ttu-id="bf81c-119">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="bf81c-119">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="bf81c-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf81c-120">Boolean</span></span>|<span data-ttu-id="bf81c-121">Se o aplicativo será ou não desinstalado quando o dispositivo for removido do Intune.</span><span class="sxs-lookup"><span data-stu-id="bf81c-121">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf81c-122">Relações</span><span class="sxs-lookup"><span data-stu-id="bf81c-122">Relationships</span></span>
<span data-ttu-id="bf81c-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bf81c-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf81c-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bf81c-124">JSON Representation</span></span>
<span data-ttu-id="bf81c-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bf81c-125">Here is a JSON representation of the resource.</span></span>
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



