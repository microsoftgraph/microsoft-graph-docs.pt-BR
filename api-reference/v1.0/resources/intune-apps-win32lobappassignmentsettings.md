---
title: tipo de recurso win32LobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel de LOB do Win32 a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7e84a740a45cb57417c81b5c99a892642097413b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020220"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="53387-103">tipo de recurso win32LobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="53387-103">win32LobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="53387-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53387-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53387-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="53387-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53387-106">Contém propriedades usadas para atribuir um aplicativo móvel de LOB do Win32 a um grupo.</span><span class="sxs-lookup"><span data-stu-id="53387-106">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="53387-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="53387-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="53387-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="53387-108">Properties</span></span>
|<span data-ttu-id="53387-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53387-109">Property</span></span>|<span data-ttu-id="53387-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="53387-110">Type</span></span>|<span data-ttu-id="53387-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="53387-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53387-112">por</span><span class="sxs-lookup"><span data-stu-id="53387-112">notifications</span></span>|[<span data-ttu-id="53387-113">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="53387-113">win32LobAppNotification</span></span>](../resources/intune-apps-win32lobappnotification.md)|<span data-ttu-id="53387-114">O status da notificação para esta atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="53387-114">The notification status for this app assignment.</span></span> <span data-ttu-id="53387-115">Os valores possíveis são: `showAll`, `showReboot`, `hideAll`.</span><span class="sxs-lookup"><span data-stu-id="53387-115">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|
|<span data-ttu-id="53387-116">restartSettings</span><span class="sxs-lookup"><span data-stu-id="53387-116">restartSettings</span></span>|[<span data-ttu-id="53387-117">win32LobAppRestartSettings</span><span class="sxs-lookup"><span data-stu-id="53387-117">win32LobAppRestartSettings</span></span>](../resources/intune-apps-win32lobapprestartsettings.md)|<span data-ttu-id="53387-118">As configurações de reinicialização a serem aplicadas para esta atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="53387-118">The reboot settings to apply for this app assignment.</span></span>|
|<span data-ttu-id="53387-119">installTimeSettings</span><span class="sxs-lookup"><span data-stu-id="53387-119">installTimeSettings</span></span>|[<span data-ttu-id="53387-120">mobileAppInstallTimeSettings</span><span class="sxs-lookup"><span data-stu-id="53387-120">mobileAppInstallTimeSettings</span></span>](../resources/intune-apps-mobileappinstalltimesettings.md)|<span data-ttu-id="53387-121">As configurações de tempo de instalação a serem aplicadas a esta atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="53387-121">The install time settings to apply for this app assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53387-122">Relações</span><span class="sxs-lookup"><span data-stu-id="53387-122">Relationships</span></span>
<span data-ttu-id="53387-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="53387-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="53387-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="53387-124">JSON Representation</span></span>
<span data-ttu-id="53387-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="53387-125">Here is a JSON representation of the resource.</span></span>
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





