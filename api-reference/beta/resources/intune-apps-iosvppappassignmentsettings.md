---
title: Tipo de recurso iosVppAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f7570108ac38b417ca4d1a5213759c071fe8492b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950456"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="e8e15-103">Tipo de recurso iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="e8e15-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="e8e15-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e8e15-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8e15-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e8e15-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8e15-106">Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="e8e15-106">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="e8e15-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="e8e15-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e8e15-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e8e15-108">Properties</span></span>
|<span data-ttu-id="e8e15-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8e15-109">Property</span></span>|<span data-ttu-id="e8e15-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8e15-110">Type</span></span>|<span data-ttu-id="e8e15-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8e15-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8e15-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="e8e15-112">useDeviceLicensing</span></span>|<span data-ttu-id="e8e15-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="e8e15-113">Boolean</span></span>|<span data-ttu-id="e8e15-114">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e8e15-114">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="e8e15-115">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="e8e15-115">vpnConfigurationId</span></span>|<span data-ttu-id="e8e15-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8e15-116">String</span></span>|<span data-ttu-id="e8e15-117">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e8e15-117">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8e15-118">Relações</span><span class="sxs-lookup"><span data-stu-id="e8e15-118">Relationships</span></span>
<span data-ttu-id="e8e15-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e8e15-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8e15-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e8e15-120">JSON Representation</span></span>
<span data-ttu-id="e8e15-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e8e15-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignmentSettings",
  "useDeviceLicensing": true,
  "vpnConfigurationId": "String"
}
```




