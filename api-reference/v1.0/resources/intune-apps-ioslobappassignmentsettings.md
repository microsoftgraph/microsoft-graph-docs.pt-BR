---
title: Tipo de recurso iosLobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.
ms.openlocfilehash: 29642e7ba4d834d4481d5bc04b0d82a7046f544d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006876"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="21a88-103">Tipo de recurso iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="21a88-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="21a88-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="21a88-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21a88-105">Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.</span><span class="sxs-lookup"><span data-stu-id="21a88-105">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>

<span data-ttu-id="21a88-106">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="21a88-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="21a88-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="21a88-107">Properties</span></span>
|<span data-ttu-id="21a88-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21a88-108">Property</span></span>|<span data-ttu-id="21a88-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="21a88-109">Type</span></span>|<span data-ttu-id="21a88-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="21a88-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21a88-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="21a88-111">vpnConfigurationId</span></span>|<span data-ttu-id="21a88-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="21a88-112">String</span></span>|<span data-ttu-id="21a88-113">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="21a88-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21a88-114">Relações</span><span class="sxs-lookup"><span data-stu-id="21a88-114">Relationships</span></span>
<span data-ttu-id="21a88-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="21a88-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="21a88-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="21a88-116">JSON Representation</span></span>
<span data-ttu-id="21a88-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="21a88-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```



