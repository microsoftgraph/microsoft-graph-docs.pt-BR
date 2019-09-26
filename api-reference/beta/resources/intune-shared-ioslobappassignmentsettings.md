---
title: Tipo de recurso iosLobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7a379e7467fb7e76a1043d73f766dace5b28a27d
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199608"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="68ddd-103">Tipo de recurso iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="68ddd-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="68ddd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="68ddd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68ddd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="68ddd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68ddd-106">Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.</span><span class="sxs-lookup"><span data-stu-id="68ddd-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="68ddd-107">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="68ddd-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="68ddd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="68ddd-108">Properties</span></span>
|<span data-ttu-id="68ddd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="68ddd-109">Property</span></span>|<span data-ttu-id="68ddd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="68ddd-110">Type</span></span>|<span data-ttu-id="68ddd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="68ddd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68ddd-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="68ddd-112">vpnConfigurationId</span></span>|<span data-ttu-id="68ddd-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="68ddd-113">String</span></span>|<span data-ttu-id="68ddd-114">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="68ddd-114">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="68ddd-115">**Apps**</span><span class="sxs-lookup"><span data-stu-id="68ddd-115">**Apps**</span></span>|
|<span data-ttu-id="68ddd-116">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="68ddd-116">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="68ddd-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="68ddd-117">Boolean</span></span>|<span data-ttu-id="68ddd-118">Se o aplicativo será ou não desinstalado quando o dispositivo for removido do Intune.</span><span class="sxs-lookup"><span data-stu-id="68ddd-118">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68ddd-119">Relações</span><span class="sxs-lookup"><span data-stu-id="68ddd-119">Relationships</span></span>
<span data-ttu-id="68ddd-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="68ddd-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68ddd-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="68ddd-121">JSON Representation</span></span>
<span data-ttu-id="68ddd-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="68ddd-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppAssignmentSettings",
  "vpnConfigurationId": "String",
  "uninstallOnDeviceRemoval": true
}
```



