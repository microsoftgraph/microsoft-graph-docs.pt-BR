---
title: tipo de recurso win32LobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel de LOB do Win32 a um grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2df6ae2cd2543aaea2c095098ea9af2e545f6f92
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004978"
---
# <a name="win32lobappassignmentsettings-resource-type"></a><span data-ttu-id="a998d-103">tipo de recurso win32LobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="a998d-103">win32LobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="a998d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a998d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a998d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a998d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a998d-106">Contém propriedades usadas para atribuir um aplicativo móvel de LOB do Win32 a um grupo.</span><span class="sxs-lookup"><span data-stu-id="a998d-106">Contains properties used to assign an Win32 LOB mobile app to a group.</span></span>


<span data-ttu-id="a998d-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="a998d-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a998d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a998d-108">Properties</span></span>
|<span data-ttu-id="a998d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a998d-109">Property</span></span>|<span data-ttu-id="a998d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a998d-110">Type</span></span>|<span data-ttu-id="a998d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a998d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a998d-112">por</span><span class="sxs-lookup"><span data-stu-id="a998d-112">notifications</span></span>|[<span data-ttu-id="a998d-113">win32LobAppNotification</span><span class="sxs-lookup"><span data-stu-id="a998d-113">win32LobAppNotification</span></span>](../resources/intune-apps-win32lobappnotification.md)|<span data-ttu-id="a998d-114">O status da notificação esta atribuição de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a998d-114">The notification status this app assignment.</span></span> <span data-ttu-id="a998d-115">Os valores possíveis são: `showAll`, `showReboot`, `hideAll`.</span><span class="sxs-lookup"><span data-stu-id="a998d-115">Possible values are: `showAll`, `showReboot`, `hideAll`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a998d-116">Relações</span><span class="sxs-lookup"><span data-stu-id="a998d-116">Relationships</span></span>
<span data-ttu-id="a998d-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a998d-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a998d-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a998d-118">JSON Representation</span></span>
<span data-ttu-id="a998d-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a998d-119">Here is a JSON representation of the resource.</span></span>
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





