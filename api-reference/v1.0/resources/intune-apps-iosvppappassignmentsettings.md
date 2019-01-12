---
title: Tipo de recurso iosVppAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e221ceb67789f9d96195a31bd7eba8f37a9df6bc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917640"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="1b2fd-103">Tipo de recurso iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="1b2fd-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="1b2fd-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1b2fd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b2fd-105">Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="1b2fd-105">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="1b2fd-106">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="1b2fd-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1b2fd-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b2fd-107">Properties</span></span>
|<span data-ttu-id="1b2fd-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b2fd-108">Property</span></span>|<span data-ttu-id="1b2fd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b2fd-109">Type</span></span>|<span data-ttu-id="1b2fd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b2fd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b2fd-111">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="1b2fd-111">useDeviceLicensing</span></span>|<span data-ttu-id="1b2fd-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="1b2fd-112">Boolean</span></span>|<span data-ttu-id="1b2fd-113">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1b2fd-113">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="1b2fd-114">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="1b2fd-114">vpnConfigurationId</span></span>|<span data-ttu-id="1b2fd-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b2fd-115">String</span></span>|<span data-ttu-id="1b2fd-116">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1b2fd-116">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b2fd-117">Relações</span><span class="sxs-lookup"><span data-stu-id="1b2fd-117">Relationships</span></span>
<span data-ttu-id="1b2fd-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1b2fd-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1b2fd-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b2fd-119">JSON Representation</span></span>
<span data-ttu-id="1b2fd-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1b2fd-120">Here is a JSON representation of the resource.</span></span>
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



