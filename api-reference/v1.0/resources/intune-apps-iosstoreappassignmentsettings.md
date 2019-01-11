---
title: Tipo de recurso iosStoreAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS Store para um grupo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 34776d6002926486baa05d0720ce1c7eeecee927
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822229"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="2df87-103">Tipo de recurso iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="2df87-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="2df87-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2df87-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2df87-105">Contém propriedades usadas para atribuir um aplicativo móvel da iOS Store para um grupo.</span><span class="sxs-lookup"><span data-stu-id="2df87-105">Contains properties used to assign an iOS Store mobile app to a group.</span></span>

<span data-ttu-id="2df87-106">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="2df87-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2df87-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2df87-107">Properties</span></span>
|<span data-ttu-id="2df87-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2df87-108">Property</span></span>|<span data-ttu-id="2df87-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2df87-109">Type</span></span>|<span data-ttu-id="2df87-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2df87-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2df87-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="2df87-111">vpnConfigurationId</span></span>|<span data-ttu-id="2df87-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2df87-112">String</span></span>|<span data-ttu-id="2df87-113">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2df87-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2df87-114">Relações</span><span class="sxs-lookup"><span data-stu-id="2df87-114">Relationships</span></span>
<span data-ttu-id="2df87-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2df87-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2df87-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2df87-116">JSON Representation</span></span>
<span data-ttu-id="2df87-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2df87-117">Here is a JSON representation of the resource.</span></span>
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



