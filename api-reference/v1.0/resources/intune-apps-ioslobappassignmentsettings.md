---
title: Tipo de recurso iosLobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 307421c7fa5bf15628fb6bb1e10d6ba36bef5705
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531220"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="a58e8-103">Tipo de recurso iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="a58e8-103">iosLobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="a58e8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a58e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a58e8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a58e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a58e8-106">Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.</span><span class="sxs-lookup"><span data-stu-id="a58e8-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="a58e8-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="a58e8-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a58e8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a58e8-108">Properties</span></span>
|<span data-ttu-id="a58e8-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a58e8-109">Property</span></span>|<span data-ttu-id="a58e8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a58e8-110">Type</span></span>|<span data-ttu-id="a58e8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a58e8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a58e8-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="a58e8-112">vpnConfigurationId</span></span>|<span data-ttu-id="a58e8-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a58e8-113">String</span></span>|<span data-ttu-id="a58e8-114">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a58e8-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a58e8-115">Relações</span><span class="sxs-lookup"><span data-stu-id="a58e8-115">Relationships</span></span>
<span data-ttu-id="a58e8-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a58e8-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a58e8-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a58e8-117">JSON Representation</span></span>
<span data-ttu-id="a58e8-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a58e8-118">Here is a JSON representation of the resource.</span></span>
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




