---
title: Tipo de recurso iosLobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bf70ac8fe90307b6445006e3f197415ef5873379
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054746"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="28c1e-103">Tipo de recurso iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="28c1e-103">iosLobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="28c1e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28c1e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28c1e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="28c1e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28c1e-106">Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.</span><span class="sxs-lookup"><span data-stu-id="28c1e-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="28c1e-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="28c1e-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="28c1e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="28c1e-108">Properties</span></span>
|<span data-ttu-id="28c1e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28c1e-109">Property</span></span>|<span data-ttu-id="28c1e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="28c1e-110">Type</span></span>|<span data-ttu-id="28c1e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="28c1e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28c1e-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="28c1e-112">vpnConfigurationId</span></span>|<span data-ttu-id="28c1e-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28c1e-113">String</span></span>|<span data-ttu-id="28c1e-114">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="28c1e-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28c1e-115">Relações</span><span class="sxs-lookup"><span data-stu-id="28c1e-115">Relationships</span></span>
<span data-ttu-id="28c1e-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="28c1e-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="28c1e-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="28c1e-117">JSON Representation</span></span>
<span data-ttu-id="28c1e-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="28c1e-118">Here is a JSON representation of the resource.</span></span>
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









