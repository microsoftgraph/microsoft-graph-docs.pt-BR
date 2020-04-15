---
title: Tipo de recurso iosVppAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 22f41ee393dea59b6773b822daa156a6a13bb9c9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474263"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="c8346-103">Tipo de recurso iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="c8346-103">iosVppAppAssignmentSettings resource type</span></span>

<span data-ttu-id="c8346-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8346-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8346-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c8346-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8346-106">Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="c8346-106">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="c8346-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="c8346-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c8346-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c8346-108">Properties</span></span>
|<span data-ttu-id="c8346-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8346-109">Property</span></span>|<span data-ttu-id="c8346-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8346-110">Type</span></span>|<span data-ttu-id="c8346-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8346-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8346-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="c8346-112">useDeviceLicensing</span></span>|<span data-ttu-id="c8346-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="c8346-113">Boolean</span></span>|<span data-ttu-id="c8346-114">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c8346-114">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="c8346-115">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="c8346-115">vpnConfigurationId</span></span>|<span data-ttu-id="c8346-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c8346-116">String</span></span>|<span data-ttu-id="c8346-117">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c8346-117">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8346-118">Relações</span><span class="sxs-lookup"><span data-stu-id="c8346-118">Relationships</span></span>
<span data-ttu-id="c8346-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c8346-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8346-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c8346-120">JSON Representation</span></span>
<span data-ttu-id="c8346-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c8346-121">Here is a JSON representation of the resource.</span></span>
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







