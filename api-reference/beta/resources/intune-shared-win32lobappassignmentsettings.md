---
title: tipo de recurso win32LobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel de LOB do Win32 a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 199a2444a814e989d1567830c400762556f7a6fe
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43436965"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="dc632-103">tipo de recurso win32LobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="dc632-103">win32LobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="dc632-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc632-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc632-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dc632-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc632-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dc632-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc632-107">Contém propriedades usadas para atribuir um aplicativo móvel de LOB do Win32 a um grupo.</span><span class="sxs-lookup"><span data-stu-id="dc632-107">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="dc632-108">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="dc632-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dc632-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dc632-109">Properties</span></span>
|<span data-ttu-id="dc632-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc632-110">Property</span></span>|<span data-ttu-id="dc632-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc632-111">Type</span></span>|<span data-ttu-id="dc632-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc632-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc632-113">por</span><span class="sxs-lookup"><span data-stu-id="dc632-113">notifications</span></span>|[<span data-ttu-id="dc632-114">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="dc632-114">win32LobAppNotification</span></span>](../resources/intune-shared-win32lobappnotification.md)|<span data-ttu-id="dc632-115">O status da notificação para esta atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dc632-115">The notification status for this app assignment.</span></span> <span data-ttu-id="dc632-116">Os valores possíveis são: `showAll`, `showReboot`, `hideAll`.</span><span class="sxs-lookup"><span data-stu-id="dc632-116">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|
|<span data-ttu-id="dc632-117">restartSettings</span><span class="sxs-lookup"><span data-stu-id="dc632-117">restartSettings</span></span>|[<span data-ttu-id="dc632-118">win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="dc632-118">win32LobAppRestartSettings</span></span>](../resources/intune-shared-win32lobapprestartsettings.md)|<span data-ttu-id="dc632-119">As configurações de reinicialização a serem aplicadas para esta atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dc632-119">The reboot settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="dc632-120">installTimeSettings</span><span class="sxs-lookup"><span data-stu-id="dc632-120">installTimeSettings</span></span>|[<span data-ttu-id="dc632-121">mobileAppInstallTimeSettings</span><span class="sxs-lookup"><span data-stu-id="dc632-121">mobileAppInstallTimeSettings</span></span>](../resources/intune-shared-mobileappinstalltimesettings.md)|<span data-ttu-id="dc632-122">As configurações de tempo de instalação a serem aplicadas a esta atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dc632-122">The install time settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="dc632-123">deliveryOptimizationPriority</span><span class="sxs-lookup"><span data-stu-id="dc632-123">deliveryOptimizationPriority</span></span>|[<span data-ttu-id="dc632-124">win32LobAppDeliveryOptimizationPriority</span><span class="sxs-lookup"><span data-stu-id="dc632-124">win32LobAppDeliveryOptimizationPriority</span></span>](../resources/intune-apps-win32lobappdeliveryoptimizationpriority.md)|<span data-ttu-id="dc632-125">A prioridade de otimização de entrega para esta atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="dc632-125">The delivery optimization priority for this app assignment.</span></span> <span data-ttu-id="dc632-126">Essa configuração não é suportada em ambientes de nuvem nacionais.</span><span class="sxs-lookup"><span data-stu-id="dc632-126">This setting is not supported in National Cloud environments.</span></span> <span data-ttu-id="dc632-127">Os valores possíveis são: `notConfigured`, `foreground`.</span><span class="sxs-lookup"><span data-stu-id="dc632-127">Possible values are: `notConfigured`, `foreground`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc632-128">Relações</span><span class="sxs-lookup"><span data-stu-id="dc632-128">Relationships</span></span>
<span data-ttu-id="dc632-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dc632-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc632-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dc632-130">JSON Representation</span></span>
<span data-ttu-id="dc632-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dc632-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppAssignmentSettings",
  "notifications": "String",
  "restartSettings": {
    "@odata.type": "microsoft.graph.win32LobAppRestartSettings",
    "gracePeriodInMinutes": 1024,
    "countdownDisplayBeforeRestartInMinutes": 1024,
    "restartNotificationSnoozeDurationInMinutes": 1024
  },
  "installTimeSettings": {
    "@odata.type": "microsoft.graph.mobileAppInstallTimeSettings",
    "useLocalTime": true,
    "startDateTime": "String (timestamp)",
    "deadlineDateTime": "String (timestamp)"
  },
  "deliveryOptimizationPriority": "String"
}
```



