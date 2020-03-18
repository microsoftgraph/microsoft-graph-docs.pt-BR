---
title: Tipo de recurso iosLobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 71dc0ff85b5b6c978a03099e863962321372f420
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42770001"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="cc3e1-103">Tipo de recurso iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="cc3e1-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="cc3e1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cc3e1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cc3e1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cc3e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc3e1-106">Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.</span><span class="sxs-lookup"><span data-stu-id="cc3e1-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="cc3e1-107">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="cc3e1-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cc3e1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cc3e1-108">Properties</span></span>
|<span data-ttu-id="cc3e1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc3e1-109">Property</span></span>|<span data-ttu-id="cc3e1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc3e1-110">Type</span></span>|<span data-ttu-id="cc3e1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc3e1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc3e1-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="cc3e1-112">vpnConfigurationId</span></span>|<span data-ttu-id="cc3e1-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc3e1-113">String</span></span>|<span data-ttu-id="cc3e1-114">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cc3e1-114">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="cc3e1-115">**Apps**</span><span class="sxs-lookup"><span data-stu-id="cc3e1-115">**Apps**</span></span>|
|<span data-ttu-id="cc3e1-116">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="cc3e1-116">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="cc3e1-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc3e1-117">Boolean</span></span>|<span data-ttu-id="cc3e1-118">Se o aplicativo será ou não desinstalado quando o dispositivo for removido do Intune.</span><span class="sxs-lookup"><span data-stu-id="cc3e1-118">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc3e1-119">Relações</span><span class="sxs-lookup"><span data-stu-id="cc3e1-119">Relationships</span></span>
<span data-ttu-id="cc3e1-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cc3e1-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc3e1-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cc3e1-121">JSON Representation</span></span>
<span data-ttu-id="cc3e1-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cc3e1-122">Here is a JSON representation of the resource.</span></span>
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



