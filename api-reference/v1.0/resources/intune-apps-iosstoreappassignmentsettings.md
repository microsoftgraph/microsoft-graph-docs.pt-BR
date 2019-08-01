---
title: Tipo de recurso iosStoreAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS Store para um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b7a0b76ff2ac66ecffc7b55e0b4d28f234cbec43
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029138"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="f4e72-103">Tipo de recurso iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="f4e72-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="f4e72-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f4e72-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4e72-105">Contém propriedades usadas para atribuir um aplicativo móvel da iOS Store para um grupo.</span><span class="sxs-lookup"><span data-stu-id="f4e72-105">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="f4e72-106">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="f4e72-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f4e72-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4e72-107">Properties</span></span>
|<span data-ttu-id="f4e72-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4e72-108">Property</span></span>|<span data-ttu-id="f4e72-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4e72-109">Type</span></span>|<span data-ttu-id="f4e72-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4e72-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4e72-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="f4e72-111">vpnConfigurationId</span></span>|<span data-ttu-id="f4e72-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f4e72-112">String</span></span>|<span data-ttu-id="f4e72-113">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f4e72-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f4e72-114">Relações</span><span class="sxs-lookup"><span data-stu-id="f4e72-114">Relationships</span></span>
<span data-ttu-id="f4e72-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f4e72-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4e72-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4e72-116">JSON Representation</span></span>
<span data-ttu-id="f4e72-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f4e72-117">Here is a JSON representation of the resource.</span></span>
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



