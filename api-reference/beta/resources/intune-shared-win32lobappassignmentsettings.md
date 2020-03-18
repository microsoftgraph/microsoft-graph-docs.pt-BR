---
title: tipo de recurso win32LobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel de LOB do Win32 a um grupo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 340dc21cce7b52ebc55c13488f7340c7b66f9e26
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42767040"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="ea7e0-103">tipo de recurso win32LobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="ea7e0-103">win32LobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="ea7e0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ea7e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea7e0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ea7e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea7e0-106">Contém propriedades usadas para atribuir um aplicativo móvel de LOB do Win32 a um grupo.</span><span class="sxs-lookup"><span data-stu-id="ea7e0-106">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="ea7e0-107">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="ea7e0-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ea7e0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea7e0-108">Properties</span></span>
|<span data-ttu-id="ea7e0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea7e0-109">Property</span></span>|<span data-ttu-id="ea7e0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea7e0-110">Type</span></span>|<span data-ttu-id="ea7e0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea7e0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea7e0-112">por</span><span class="sxs-lookup"><span data-stu-id="ea7e0-112">notifications</span></span>|[<span data-ttu-id="ea7e0-113">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="ea7e0-113">win32LobAppNotification</span></span>](../resources/intune-shared-win32lobappnotification.md)|<span data-ttu-id="ea7e0-114">O status da notificação para esta atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ea7e0-114">The notification status for this app assignment.</span></span> <span data-ttu-id="ea7e0-115">Os valores possíveis são: `showAll`, `showReboot`, `hideAll`.</span><span class="sxs-lookup"><span data-stu-id="ea7e0-115">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|
|<span data-ttu-id="ea7e0-116">restartSettings</span><span class="sxs-lookup"><span data-stu-id="ea7e0-116">restartSettings</span></span>|[<span data-ttu-id="ea7e0-117">win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="ea7e0-117">win32LobAppRestartSettings</span></span>](../resources/intune-shared-win32lobapprestartsettings.md)|<span data-ttu-id="ea7e0-118">As configurações de reinicialização a serem aplicadas para esta atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ea7e0-118">The reboot settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="ea7e0-119">installTimeSettings</span><span class="sxs-lookup"><span data-stu-id="ea7e0-119">installTimeSettings</span></span>|[<span data-ttu-id="ea7e0-120">mobileAppInstallTimeSettings</span><span class="sxs-lookup"><span data-stu-id="ea7e0-120">mobileAppInstallTimeSettings</span></span>](../resources/intune-shared-mobileappinstalltimesettings.md)|<span data-ttu-id="ea7e0-121">As configurações de tempo de instalação a serem aplicadas a esta atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ea7e0-121">The install time settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="ea7e0-122">deliveryOptimizationPriority</span><span class="sxs-lookup"><span data-stu-id="ea7e0-122">deliveryOptimizationPriority</span></span>|[<span data-ttu-id="ea7e0-123">win32LobAppDeliveryOptimizationPriority</span><span class="sxs-lookup"><span data-stu-id="ea7e0-123">win32LobAppDeliveryOptimizationPriority</span></span>](../resources/intune-apps-win32lobappdeliveryoptimizationpriority.md)|<span data-ttu-id="ea7e0-124">A prioridade de otimização de entrega para esta atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ea7e0-124">The delivery optimization priority for this app assignment.</span></span> <span data-ttu-id="ea7e0-125">Essa configuração não é suportada em ambientes de nuvem nacionais.</span><span class="sxs-lookup"><span data-stu-id="ea7e0-125">This setting is not supported in National Cloud environments.</span></span> <span data-ttu-id="ea7e0-126">Os valores possíveis são: `notConfigured`, `foreground`.</span><span class="sxs-lookup"><span data-stu-id="ea7e0-126">Possible values are: `notConfigured`, `foreground`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea7e0-127">Relações</span><span class="sxs-lookup"><span data-stu-id="ea7e0-127">Relationships</span></span>
<span data-ttu-id="ea7e0-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea7e0-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea7e0-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea7e0-129">JSON Representation</span></span>
<span data-ttu-id="ea7e0-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea7e0-130">Here is a JSON representation of the resource.</span></span>
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



