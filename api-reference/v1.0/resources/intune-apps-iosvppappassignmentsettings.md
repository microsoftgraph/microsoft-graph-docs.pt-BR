---
title: Tipo de recurso iosVppAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 883f81ab29dd2258d57753b792f0a4f1f434ed43
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360206"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="e995f-103">Tipo de recurso iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="e995f-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="e995f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e995f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e995f-105">Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="e995f-105">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="e995f-106">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="e995f-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e995f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e995f-107">Properties</span></span>
|<span data-ttu-id="e995f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e995f-108">Property</span></span>|<span data-ttu-id="e995f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e995f-109">Type</span></span>|<span data-ttu-id="e995f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e995f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e995f-111">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="e995f-111">useDeviceLicensing</span></span>|<span data-ttu-id="e995f-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="e995f-112">Boolean</span></span>|<span data-ttu-id="e995f-113">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e995f-113">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="e995f-114">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="e995f-114">vpnConfigurationId</span></span>|<span data-ttu-id="e995f-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e995f-115">String</span></span>|<span data-ttu-id="e995f-116">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e995f-116">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e995f-117">Relações</span><span class="sxs-lookup"><span data-stu-id="e995f-117">Relationships</span></span>
<span data-ttu-id="e995f-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e995f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e995f-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e995f-119">JSON Representation</span></span>
<span data-ttu-id="e995f-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e995f-120">Here is a JSON representation of the resource.</span></span>
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




