---
title: tipo de recurso win32LobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel de LOB do Win32 a um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 445cd1a03a7495d4946f600dea3773d7bd9e2249
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774236"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="1cb09-103">tipo de recurso win32LobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="1cb09-103">win32LobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="1cb09-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1cb09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1cb09-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1cb09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1cb09-106">Contém propriedades usadas para atribuir um aplicativo móvel de LOB do Win32 a um grupo.</span><span class="sxs-lookup"><span data-stu-id="1cb09-106">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="1cb09-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="1cb09-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1cb09-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1cb09-108">Properties</span></span>
|<span data-ttu-id="1cb09-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1cb09-109">Property</span></span>|<span data-ttu-id="1cb09-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cb09-110">Type</span></span>|<span data-ttu-id="1cb09-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cb09-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cb09-112">por</span><span class="sxs-lookup"><span data-stu-id="1cb09-112">notifications</span></span>|[<span data-ttu-id="1cb09-113">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="1cb09-113">win32LobAppNotification</span></span>](../resources/intune-apps-win32lobappnotification.md)|<span data-ttu-id="1cb09-114">O status da notificação esta atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1cb09-114">The notification status this app assignment.</span></span> <span data-ttu-id="1cb09-115">Os valores possíveis são: `showAll`, `showReboot`, `hideAll`.</span><span class="sxs-lookup"><span data-stu-id="1cb09-115">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1cb09-116">Relações</span><span class="sxs-lookup"><span data-stu-id="1cb09-116">Relationships</span></span>
<span data-ttu-id="1cb09-117">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="1cb09-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1cb09-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1cb09-118">JSON Representation</span></span>
<span data-ttu-id="1cb09-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1cb09-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppAssignmentSettings",
  "notifications": "String"
}
```





