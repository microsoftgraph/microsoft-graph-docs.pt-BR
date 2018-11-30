---
title: Tipo de recurso iosVppAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.
ms.openlocfilehash: 6fc529fe1aeea6bdbef46ad0cd97fb5830250b4c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006489"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="4dbf4-103">Tipo de recurso iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="4dbf4-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="4dbf4-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4dbf4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4dbf4-105">Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="4dbf4-105">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="4dbf4-106">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="4dbf4-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4dbf4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4dbf4-107">Properties</span></span>
|<span data-ttu-id="4dbf4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4dbf4-108">Property</span></span>|<span data-ttu-id="4dbf4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4dbf4-109">Type</span></span>|<span data-ttu-id="4dbf4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4dbf4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dbf4-111">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="4dbf4-111">useDeviceLicensing</span></span>|<span data-ttu-id="4dbf4-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="4dbf4-112">Boolean</span></span>|<span data-ttu-id="4dbf4-113">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4dbf4-113">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="4dbf4-114">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="4dbf4-114">vpnConfigurationId</span></span>|<span data-ttu-id="4dbf4-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4dbf4-115">String</span></span>|<span data-ttu-id="4dbf4-116">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4dbf4-116">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4dbf4-117">Relações</span><span class="sxs-lookup"><span data-stu-id="4dbf4-117">Relationships</span></span>
<span data-ttu-id="4dbf4-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4dbf4-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4dbf4-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4dbf4-119">JSON Representation</span></span>
<span data-ttu-id="4dbf4-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4dbf4-120">Here is a JSON representation of the resource.</span></span>
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



