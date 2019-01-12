---
title: Tipo de recurso iosLobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 39f007a88fc05504fc83b624a886c719ffe08ba3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962267"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="0f41e-103">Tipo de recurso iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="0f41e-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="0f41e-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0f41e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f41e-105">Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.</span><span class="sxs-lookup"><span data-stu-id="0f41e-105">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>

<span data-ttu-id="0f41e-106">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="0f41e-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0f41e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0f41e-107">Properties</span></span>
|<span data-ttu-id="0f41e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f41e-108">Property</span></span>|<span data-ttu-id="0f41e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f41e-109">Type</span></span>|<span data-ttu-id="0f41e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f41e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f41e-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="0f41e-111">vpnConfigurationId</span></span>|<span data-ttu-id="0f41e-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f41e-112">String</span></span>|<span data-ttu-id="0f41e-113">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f41e-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f41e-114">Relações</span><span class="sxs-lookup"><span data-stu-id="0f41e-114">Relationships</span></span>
<span data-ttu-id="0f41e-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0f41e-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0f41e-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0f41e-116">JSON Representation</span></span>
<span data-ttu-id="0f41e-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0f41e-117">Here is a JSON representation of the resource.</span></span>
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



