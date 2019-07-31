---
title: Tipo de recurso iosLobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 539c1974505e248bc700a9d804d06c6f8bc4b257
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005531"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="288e9-103">Tipo de recurso iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="288e9-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="288e9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="288e9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="288e9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="288e9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="288e9-106">Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.</span><span class="sxs-lookup"><span data-stu-id="288e9-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="288e9-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="288e9-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="288e9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="288e9-108">Properties</span></span>
|<span data-ttu-id="288e9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="288e9-109">Property</span></span>|<span data-ttu-id="288e9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="288e9-110">Type</span></span>|<span data-ttu-id="288e9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="288e9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="288e9-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="288e9-112">vpnConfigurationId</span></span>|<span data-ttu-id="288e9-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="288e9-113">String</span></span>|<span data-ttu-id="288e9-114">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="288e9-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="288e9-115">Relações</span><span class="sxs-lookup"><span data-stu-id="288e9-115">Relationships</span></span>
<span data-ttu-id="288e9-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="288e9-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="288e9-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="288e9-117">JSON Representation</span></span>
<span data-ttu-id="288e9-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="288e9-118">Here is a JSON representation of the resource.</span></span>
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





