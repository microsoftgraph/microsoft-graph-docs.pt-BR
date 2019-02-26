---
title: Tipo de recurso iosLobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5beacfd60eb2237ed85a95bca21c27a38f956d16
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255203"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="1b910-103">Tipo de recurso iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="1b910-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="1b910-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1b910-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b910-105">Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.</span><span class="sxs-lookup"><span data-stu-id="1b910-105">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="1b910-106">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="1b910-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1b910-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1b910-107">Properties</span></span>
|<span data-ttu-id="1b910-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1b910-108">Property</span></span>|<span data-ttu-id="1b910-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1b910-109">Type</span></span>|<span data-ttu-id="1b910-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b910-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b910-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="1b910-111">vpnConfigurationId</span></span>|<span data-ttu-id="1b910-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1b910-112">String</span></span>|<span data-ttu-id="1b910-113">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1b910-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b910-114">Relações</span><span class="sxs-lookup"><span data-stu-id="1b910-114">Relationships</span></span>
<span data-ttu-id="1b910-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1b910-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b910-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1b910-116">JSON Representation</span></span>
<span data-ttu-id="1b910-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1b910-117">Here is a JSON representation of the resource.</span></span>
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



