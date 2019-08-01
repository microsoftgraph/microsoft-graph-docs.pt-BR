---
title: Tipo de recurso iosVppAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d35cd60b1e616f38b8c4c792f7bd766f550b62aa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029117"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="22158-103">Tipo de recurso iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="22158-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="22158-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="22158-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22158-105">Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="22158-105">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="22158-106">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="22158-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="22158-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="22158-107">Properties</span></span>
|<span data-ttu-id="22158-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22158-108">Property</span></span>|<span data-ttu-id="22158-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="22158-109">Type</span></span>|<span data-ttu-id="22158-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="22158-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22158-111">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="22158-111">useDeviceLicensing</span></span>|<span data-ttu-id="22158-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="22158-112">Boolean</span></span>|<span data-ttu-id="22158-113">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="22158-113">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="22158-114">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="22158-114">vpnConfigurationId</span></span>|<span data-ttu-id="22158-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22158-115">String</span></span>|<span data-ttu-id="22158-116">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="22158-116">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22158-117">Relações</span><span class="sxs-lookup"><span data-stu-id="22158-117">Relationships</span></span>
<span data-ttu-id="22158-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="22158-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="22158-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="22158-119">JSON Representation</span></span>
<span data-ttu-id="22158-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="22158-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignmentSettings",
  "useDeviceLicensing": true,
  "vpnConfigurationId": "String"
}
```



