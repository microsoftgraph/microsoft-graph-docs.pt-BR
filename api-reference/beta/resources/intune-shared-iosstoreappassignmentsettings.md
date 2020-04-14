---
title: Tipo de recurso iosStoreAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS Store para um grupo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 41ebc66736b5a21dc052cd089e3abd05ae00b37b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460606"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="99672-103">Tipo de recurso iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="99672-103">iosStoreAppAssignmentSettings resource type</span></span>

<span data-ttu-id="99672-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99672-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99672-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="99672-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99672-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="99672-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99672-107">Contém propriedades usadas para atribuir um aplicativo móvel da iOS Store para um grupo.</span><span class="sxs-lookup"><span data-stu-id="99672-107">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="99672-108">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="99672-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="99672-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99672-109">Properties</span></span>
|<span data-ttu-id="99672-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99672-110">Property</span></span>|<span data-ttu-id="99672-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="99672-111">Type</span></span>|<span data-ttu-id="99672-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="99672-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99672-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="99672-113">vpnConfigurationId</span></span>|<span data-ttu-id="99672-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99672-114">String</span></span>|<span data-ttu-id="99672-115">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="99672-115">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="99672-116">**Apps**</span><span class="sxs-lookup"><span data-stu-id="99672-116">**Apps**</span></span>|
|<span data-ttu-id="99672-117">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="99672-117">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="99672-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="99672-118">Boolean</span></span>|<span data-ttu-id="99672-119">Se o aplicativo será ou não desinstalado quando o dispositivo for removido do Intune.</span><span class="sxs-lookup"><span data-stu-id="99672-119">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99672-120">Relações</span><span class="sxs-lookup"><span data-stu-id="99672-120">Relationships</span></span>
<span data-ttu-id="99672-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="99672-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99672-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99672-122">JSON Representation</span></span>
<span data-ttu-id="99672-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="99672-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosStoreAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosStoreAppAssignmentSettings",
  "vpnConfigurationId": "String",
  "uninstallOnDeviceRemoval": true
}
```



