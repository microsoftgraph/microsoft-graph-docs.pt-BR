---
title: tipo de recurso win32LobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel de LOB do Win32 a um grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e1f650919e3e7cd9fa55d7e05d3fc706b18f95db
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538690"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="b6c4d-103">tipo de recurso win32LobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="b6c4d-103">win32LobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="b6c4d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b6c4d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6c4d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b6c4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6c4d-106">Contém propriedades usadas para atribuir um aplicativo móvel de LOB do Win32 a um grupo.</span><span class="sxs-lookup"><span data-stu-id="b6c4d-106">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="b6c4d-107">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="b6c4d-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b6c4d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b6c4d-108">Properties</span></span>
|<span data-ttu-id="b6c4d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6c4d-109">Property</span></span>|<span data-ttu-id="b6c4d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6c4d-110">Type</span></span>|<span data-ttu-id="b6c4d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6c4d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6c4d-112">por</span><span class="sxs-lookup"><span data-stu-id="b6c4d-112">notifications</span></span>|[<span data-ttu-id="b6c4d-113">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="b6c4d-113">win32LobAppNotification</span></span>](../resources/intune-shared-win32lobappnotification.md)|<span data-ttu-id="b6c4d-114">O status da notificação para esta atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b6c4d-114">The notification status for this app assignment.</span></span> <span data-ttu-id="b6c4d-115">Os valores possíveis são: `showAll`, `showReboot`, `hideAll`.</span><span class="sxs-lookup"><span data-stu-id="b6c4d-115">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|
|<span data-ttu-id="b6c4d-116">restartSettings</span><span class="sxs-lookup"><span data-stu-id="b6c4d-116">restartSettings</span></span>|[<span data-ttu-id="b6c4d-117">win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="b6c4d-117">win32LobAppRestartSettings</span></span>](../resources/intune-shared-win32lobapprestartsettings.md)|<span data-ttu-id="b6c4d-118">As configurações de reinicialização a serem aplicadas para esta atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b6c4d-118">The reboot settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="b6c4d-119">installTimeSettings</span><span class="sxs-lookup"><span data-stu-id="b6c4d-119">installTimeSettings</span></span>|[<span data-ttu-id="b6c4d-120">mobileAppInstallTimeSettings</span><span class="sxs-lookup"><span data-stu-id="b6c4d-120">mobileAppInstallTimeSettings</span></span>](../resources/intune-shared-mobileappinstalltimesettings.md)|<span data-ttu-id="b6c4d-121">As configurações de tempo de instalação a serem aplicadas a esta atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b6c4d-121">The install time settings to apply for this app assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6c4d-122">Relações</span><span class="sxs-lookup"><span data-stu-id="b6c4d-122">Relationships</span></span>
<span data-ttu-id="b6c4d-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b6c4d-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6c4d-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b6c4d-124">JSON Representation</span></span>
<span data-ttu-id="b6c4d-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b6c4d-125">Here is a JSON representation of the resource.</span></span>
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
  }
}
```



