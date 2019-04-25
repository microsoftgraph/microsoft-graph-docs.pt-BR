---
title: Tipo de recurso iosStoreAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS Store para um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d58490e97aec48f664ab6882198e4c1da3511e8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523942"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="7d1cc-103">Tipo de recurso iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="7d1cc-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="7d1cc-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7d1cc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d1cc-105">Contém propriedades usadas para atribuir um aplicativo móvel da iOS Store para um grupo.</span><span class="sxs-lookup"><span data-stu-id="7d1cc-105">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="7d1cc-106">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="7d1cc-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7d1cc-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7d1cc-107">Properties</span></span>
|<span data-ttu-id="7d1cc-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d1cc-108">Property</span></span>|<span data-ttu-id="7d1cc-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d1cc-109">Type</span></span>|<span data-ttu-id="7d1cc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d1cc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d1cc-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="7d1cc-111">vpnConfigurationId</span></span>|<span data-ttu-id="7d1cc-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d1cc-112">String</span></span>|<span data-ttu-id="7d1cc-113">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7d1cc-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d1cc-114">Relações</span><span class="sxs-lookup"><span data-stu-id="7d1cc-114">Relationships</span></span>
<span data-ttu-id="7d1cc-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7d1cc-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d1cc-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7d1cc-116">JSON Representation</span></span>
<span data-ttu-id="7d1cc-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7d1cc-117">Here is a JSON representation of the resource.</span></span>
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



