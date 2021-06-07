---
title: Tipo de recurso win32LobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel LOB win32 a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d76e189d684999e3922b625def26d4d0cfcb6a3e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752207"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="140a6-103">Tipo de recurso win32LobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="140a6-103">win32LobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="140a6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="140a6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="140a6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="140a6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="140a6-106">Contém propriedades usadas para atribuir um aplicativo móvel LOB win32 a um grupo.</span><span class="sxs-lookup"><span data-stu-id="140a6-106">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="140a6-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="140a6-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="140a6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="140a6-108">Properties</span></span>
|<span data-ttu-id="140a6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="140a6-109">Property</span></span>|<span data-ttu-id="140a6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="140a6-110">Type</span></span>|<span data-ttu-id="140a6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="140a6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="140a6-112">notificações</span><span class="sxs-lookup"><span data-stu-id="140a6-112">notifications</span></span>|[<span data-ttu-id="140a6-113">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="140a6-113">win32LobAppNotification</span></span>](../resources/intune-apps-win32lobappnotification.md)|<span data-ttu-id="140a6-114">O status de notificação para essa atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="140a6-114">The notification status for this app assignment.</span></span> <span data-ttu-id="140a6-115">Os valores possíveis são: `showAll`, `showReboot`, `hideAll`.</span><span class="sxs-lookup"><span data-stu-id="140a6-115">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|
|<span data-ttu-id="140a6-116">restartSettings</span><span class="sxs-lookup"><span data-stu-id="140a6-116">restartSettings</span></span>|[<span data-ttu-id="140a6-117">win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="140a6-117">win32LobAppRestartSettings</span></span>](../resources/intune-apps-win32lobapprestartsettings.md)|<span data-ttu-id="140a6-118">As configurações de reinicialização a ser aplicadas a essa atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="140a6-118">The reboot settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="140a6-119">installTimeSettings</span><span class="sxs-lookup"><span data-stu-id="140a6-119">installTimeSettings</span></span>|[<span data-ttu-id="140a6-120">mobileAppInstallTimeSettings</span><span class="sxs-lookup"><span data-stu-id="140a6-120">mobileAppInstallTimeSettings</span></span>](../resources/intune-apps-mobileappinstalltimesettings.md)|<span data-ttu-id="140a6-121">As configurações de tempo de instalação a ser aplicadas a essa atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="140a6-121">The install time settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="140a6-122">deliveryOptimizationPriority</span><span class="sxs-lookup"><span data-stu-id="140a6-122">deliveryOptimizationPriority</span></span>|[<span data-ttu-id="140a6-123">win32LobAppDeliveryOptimizationPriority</span><span class="sxs-lookup"><span data-stu-id="140a6-123">win32LobAppDeliveryOptimizationPriority</span></span>](../resources/intune-apps-win32lobappdeliveryoptimizationpriority.md)|<span data-ttu-id="140a6-124">A prioridade de otimização de entrega para essa atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="140a6-124">The delivery optimization priority for this app assignment.</span></span> <span data-ttu-id="140a6-125">Essa configuração não é suportada em ambientes de Nuvem Nacional.</span><span class="sxs-lookup"><span data-stu-id="140a6-125">This setting is not supported in National Cloud environments.</span></span> <span data-ttu-id="140a6-126">Os valores possíveis são: `notConfigured`, `foreground`.</span><span class="sxs-lookup"><span data-stu-id="140a6-126">Possible values are: `notConfigured`, `foreground`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="140a6-127">Relações</span><span class="sxs-lookup"><span data-stu-id="140a6-127">Relationships</span></span>
<span data-ttu-id="140a6-128">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="140a6-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="140a6-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="140a6-129">JSON Representation</span></span>
<span data-ttu-id="140a6-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="140a6-130">Here is a JSON representation of the resource.</span></span>
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




