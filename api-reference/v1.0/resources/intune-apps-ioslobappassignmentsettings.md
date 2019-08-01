---
title: Tipo de recurso iosLobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8cb033283c163a30dbedf7088001025c327dbae6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029162"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="1ce57-103">Tipo de recurso iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="1ce57-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="1ce57-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1ce57-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ce57-105">Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.</span><span class="sxs-lookup"><span data-stu-id="1ce57-105">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="1ce57-106">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="1ce57-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1ce57-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ce57-107">Properties</span></span>
|<span data-ttu-id="1ce57-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ce57-108">Property</span></span>|<span data-ttu-id="1ce57-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ce57-109">Type</span></span>|<span data-ttu-id="1ce57-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ce57-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ce57-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="1ce57-111">vpnConfigurationId</span></span>|<span data-ttu-id="1ce57-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ce57-112">String</span></span>|<span data-ttu-id="1ce57-113">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1ce57-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ce57-114">Relações</span><span class="sxs-lookup"><span data-stu-id="1ce57-114">Relationships</span></span>
<span data-ttu-id="1ce57-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1ce57-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ce57-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ce57-116">JSON Representation</span></span>
<span data-ttu-id="1ce57-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1ce57-117">Here is a JSON representation of the resource.</span></span>
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



