---
title: Tipo de recurso iosVppAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.
author: tfitzmac
ms.openlocfilehash: 65a143c1f6cc9eed4dfdc6dabeb6f9379517277c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310245"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="6a1ee-103">Tipo de recurso iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="6a1ee-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="6a1ee-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6a1ee-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a1ee-105">Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="6a1ee-105">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="6a1ee-106">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="6a1ee-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6a1ee-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a1ee-107">Properties</span></span>
|<span data-ttu-id="6a1ee-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a1ee-108">Property</span></span>|<span data-ttu-id="6a1ee-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a1ee-109">Type</span></span>|<span data-ttu-id="6a1ee-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a1ee-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a1ee-111">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="6a1ee-111">useDeviceLicensing</span></span>|<span data-ttu-id="6a1ee-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a1ee-112">Boolean</span></span>|<span data-ttu-id="6a1ee-113">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6a1ee-113">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="6a1ee-114">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="6a1ee-114">vpnConfigurationId</span></span>|<span data-ttu-id="6a1ee-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a1ee-115">String</span></span>|<span data-ttu-id="6a1ee-116">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6a1ee-116">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a1ee-117">Relações</span><span class="sxs-lookup"><span data-stu-id="6a1ee-117">Relationships</span></span>
<span data-ttu-id="6a1ee-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a1ee-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6a1ee-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a1ee-119">JSON Representation</span></span>
<span data-ttu-id="6a1ee-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6a1ee-120">Here is a JSON representation of the resource.</span></span>
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



