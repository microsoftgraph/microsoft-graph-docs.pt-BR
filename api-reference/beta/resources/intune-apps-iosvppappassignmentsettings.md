---
title: Tipo de recurso iosVppAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36c6e2c60423038f2af10ccdbcfaf94ecd6ec3aa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552321"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="f0d56-103">Tipo de recurso iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="f0d56-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="f0d56-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f0d56-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0d56-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f0d56-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0d56-106">Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="f0d56-106">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="f0d56-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="f0d56-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f0d56-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f0d56-108">Properties</span></span>
|<span data-ttu-id="f0d56-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0d56-109">Property</span></span>|<span data-ttu-id="f0d56-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0d56-110">Type</span></span>|<span data-ttu-id="f0d56-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0d56-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0d56-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="f0d56-112">useDeviceLicensing</span></span>|<span data-ttu-id="f0d56-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="f0d56-113">Boolean</span></span>|<span data-ttu-id="f0d56-114">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f0d56-114">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="f0d56-115">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="f0d56-115">vpnConfigurationId</span></span>|<span data-ttu-id="f0d56-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0d56-116">String</span></span>|<span data-ttu-id="f0d56-117">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f0d56-117">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0d56-118">Relações</span><span class="sxs-lookup"><span data-stu-id="f0d56-118">Relationships</span></span>
<span data-ttu-id="f0d56-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f0d56-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0d56-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f0d56-120">JSON Representation</span></span>
<span data-ttu-id="f0d56-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f0d56-121">Here is a JSON representation of the resource.</span></span>
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





