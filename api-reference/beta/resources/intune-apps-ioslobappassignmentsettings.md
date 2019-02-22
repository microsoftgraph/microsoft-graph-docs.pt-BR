---
title: Tipo de recurso iosLobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c8f1dadc7a302c3b4b78f0fc9e278e9285ecbcc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172307"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="86069-103">Tipo de recurso iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="86069-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="86069-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="86069-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86069-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="86069-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86069-106">Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.</span><span class="sxs-lookup"><span data-stu-id="86069-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="86069-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="86069-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="86069-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="86069-108">Properties</span></span>
|<span data-ttu-id="86069-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86069-109">Property</span></span>|<span data-ttu-id="86069-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="86069-110">Type</span></span>|<span data-ttu-id="86069-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="86069-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86069-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="86069-112">vpnConfigurationId</span></span>|<span data-ttu-id="86069-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86069-113">String</span></span>|<span data-ttu-id="86069-114">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="86069-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86069-115">Relações</span><span class="sxs-lookup"><span data-stu-id="86069-115">Relationships</span></span>
<span data-ttu-id="86069-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="86069-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="86069-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="86069-117">JSON Representation</span></span>
<span data-ttu-id="86069-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="86069-118">Here is a JSON representation of the resource.</span></span>
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




