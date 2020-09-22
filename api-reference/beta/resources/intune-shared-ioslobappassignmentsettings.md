---
title: Tipo de recurso iosLobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8168e8c9a5626d305594d5f302ec99e59de89614
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084237"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="76d52-103">Tipo de recurso iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="76d52-103">iosLobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="76d52-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76d52-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76d52-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="76d52-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76d52-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="76d52-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76d52-107">Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.</span><span class="sxs-lookup"><span data-stu-id="76d52-107">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="76d52-108">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="76d52-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="76d52-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="76d52-109">Properties</span></span>
|<span data-ttu-id="76d52-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76d52-110">Property</span></span>|<span data-ttu-id="76d52-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="76d52-111">Type</span></span>|<span data-ttu-id="76d52-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="76d52-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76d52-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="76d52-113">vpnConfigurationId</span></span>|<span data-ttu-id="76d52-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76d52-114">String</span></span>|<span data-ttu-id="76d52-115">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="76d52-115">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="76d52-116">**Aplicativos**</span><span class="sxs-lookup"><span data-stu-id="76d52-116">**Apps**</span></span>|
|<span data-ttu-id="76d52-117">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="76d52-117">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="76d52-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="76d52-118">Boolean</span></span>|<span data-ttu-id="76d52-119">Se o aplicativo será ou não desinstalado quando o dispositivo for removido do Intune.</span><span class="sxs-lookup"><span data-stu-id="76d52-119">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76d52-120">Relações</span><span class="sxs-lookup"><span data-stu-id="76d52-120">Relationships</span></span>
<span data-ttu-id="76d52-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="76d52-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="76d52-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="76d52-122">JSON Representation</span></span>
<span data-ttu-id="76d52-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="76d52-123">Here is a JSON representation of the resource.</span></span>
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






