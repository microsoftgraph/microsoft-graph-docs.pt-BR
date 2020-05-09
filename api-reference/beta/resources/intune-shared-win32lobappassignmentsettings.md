---
title: tipo de recurso win32LobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel de LOB do Win32 a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 53872d032bbb61cf57d191f1b58f1878ba5c0a91
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177657"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="2c6e6-103">tipo de recurso win32LobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="2c6e6-103">win32LobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="2c6e6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c6e6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2c6e6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c6e6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c6e6-107">Contém propriedades usadas para atribuir um aplicativo móvel de LOB do Win32 a um grupo.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-107">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="2c6e6-108">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="2c6e6-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2c6e6-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c6e6-109">Properties</span></span>
|<span data-ttu-id="2c6e6-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c6e6-110">Property</span></span>|<span data-ttu-id="2c6e6-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c6e6-111">Type</span></span>|<span data-ttu-id="2c6e6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c6e6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c6e6-113">por</span><span class="sxs-lookup"><span data-stu-id="2c6e6-113">notifications</span></span>|[<span data-ttu-id="2c6e6-114">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="2c6e6-114">win32LobAppNotification</span></span>](../resources/intune-shared-win32lobappnotification.md)|<span data-ttu-id="2c6e6-115">O status da notificação para esta atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-115">The notification status for this app assignment.</span></span> <span data-ttu-id="2c6e6-116">Os valores possíveis são: `showAll`, `showReboot`, `hideAll`.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-116">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|
|<span data-ttu-id="2c6e6-117">restartSettings</span><span class="sxs-lookup"><span data-stu-id="2c6e6-117">restartSettings</span></span>|[<span data-ttu-id="2c6e6-118">win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="2c6e6-118">win32LobAppRestartSettings</span></span>](../resources/intune-shared-win32lobapprestartsettings.md)|<span data-ttu-id="2c6e6-119">As configurações de reinicialização a serem aplicadas para esta atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-119">The reboot settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="2c6e6-120">installTimeSettings</span><span class="sxs-lookup"><span data-stu-id="2c6e6-120">installTimeSettings</span></span>|[<span data-ttu-id="2c6e6-121">mobileAppInstallTimeSettings</span><span class="sxs-lookup"><span data-stu-id="2c6e6-121">mobileAppInstallTimeSettings</span></span>](../resources/intune-shared-mobileappinstalltimesettings.md)|<span data-ttu-id="2c6e6-122">As configurações de tempo de instalação a serem aplicadas a esta atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-122">The install time settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="2c6e6-123">deliveryOptimizationPriority</span><span class="sxs-lookup"><span data-stu-id="2c6e6-123">deliveryOptimizationPriority</span></span>|[<span data-ttu-id="2c6e6-124">win32LobAppDeliveryOptimizationPriority</span><span class="sxs-lookup"><span data-stu-id="2c6e6-124">win32LobAppDeliveryOptimizationPriority</span></span>](../resources/intune-shared-win32lobappdeliveryoptimizationpriority.md)|<span data-ttu-id="2c6e6-125">A prioridade de otimização de entrega para esta atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-125">The delivery optimization priority for this app assignment.</span></span> <span data-ttu-id="2c6e6-126">Essa configuração não é suportada em ambientes de nuvem nacionais.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-126">This setting is not supported in National Cloud environments.</span></span> <span data-ttu-id="2c6e6-127">Os valores possíveis são: `notConfigured`, `foreground`.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-127">Possible values are: `notConfigured`, `foreground`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c6e6-128">Relações</span><span class="sxs-lookup"><span data-stu-id="2c6e6-128">Relationships</span></span>
<span data-ttu-id="2c6e6-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2c6e6-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c6e6-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c6e6-130">JSON Representation</span></span>
<span data-ttu-id="2c6e6-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c6e6-131">Here is a JSON representation of the resource.</span></span>
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



