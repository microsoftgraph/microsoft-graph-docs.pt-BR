---
title: Tipo de recurso iosStoreAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS Store para um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dcda842b97c6c7baf257145f0333c6194e97a403
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31806423"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="a81c3-103">Tipo de recurso iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="a81c3-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="a81c3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a81c3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a81c3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a81c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a81c3-106">Contém propriedades usadas para atribuir um aplicativo móvel da iOS Store para um grupo.</span><span class="sxs-lookup"><span data-stu-id="a81c3-106">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="a81c3-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="a81c3-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a81c3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a81c3-108">Properties</span></span>
|<span data-ttu-id="a81c3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a81c3-109">Property</span></span>|<span data-ttu-id="a81c3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a81c3-110">Type</span></span>|<span data-ttu-id="a81c3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a81c3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a81c3-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="a81c3-112">vpnConfigurationId</span></span>|<span data-ttu-id="a81c3-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a81c3-113">String</span></span>|<span data-ttu-id="a81c3-114">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a81c3-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a81c3-115">Relações</span><span class="sxs-lookup"><span data-stu-id="a81c3-115">Relationships</span></span>
<span data-ttu-id="a81c3-116">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="a81c3-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a81c3-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a81c3-117">JSON Representation</span></span>
<span data-ttu-id="a81c3-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a81c3-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosStoreAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosStoreAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```





