---
title: Tipo de recurso iosLobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 48bac2fcc8dd8c7da65c3ee138aabaaf5649b356
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31795181"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="0f873-103">Tipo de recurso iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="0f873-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="0f873-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0f873-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f873-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0f873-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f873-106">Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.</span><span class="sxs-lookup"><span data-stu-id="0f873-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="0f873-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="0f873-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0f873-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0f873-108">Properties</span></span>
|<span data-ttu-id="0f873-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0f873-109">Property</span></span>|<span data-ttu-id="0f873-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0f873-110">Type</span></span>|<span data-ttu-id="0f873-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f873-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f873-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="0f873-112">vpnConfigurationId</span></span>|<span data-ttu-id="0f873-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0f873-113">String</span></span>|<span data-ttu-id="0f873-114">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0f873-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f873-115">Relações</span><span class="sxs-lookup"><span data-stu-id="0f873-115">Relationships</span></span>
<span data-ttu-id="0f873-116">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="0f873-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f873-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0f873-117">JSON Representation</span></span>
<span data-ttu-id="0f873-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0f873-118">Here is a JSON representation of the resource.</span></span>
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





