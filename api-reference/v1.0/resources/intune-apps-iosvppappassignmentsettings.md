---
title: Tipo de recurso iosVppAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d1ff346b9ae786fdc2158a5386625f808e04c181
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523907"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="1a2ca-103">Tipo de recurso iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="1a2ca-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="1a2ca-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1a2ca-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a2ca-105">Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="1a2ca-105">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="1a2ca-106">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="1a2ca-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1a2ca-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a2ca-107">Properties</span></span>
|<span data-ttu-id="1a2ca-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a2ca-108">Property</span></span>|<span data-ttu-id="1a2ca-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a2ca-109">Type</span></span>|<span data-ttu-id="1a2ca-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a2ca-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a2ca-111">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="1a2ca-111">useDeviceLicensing</span></span>|<span data-ttu-id="1a2ca-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="1a2ca-112">Boolean</span></span>|<span data-ttu-id="1a2ca-113">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1a2ca-113">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="1a2ca-114">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="1a2ca-114">vpnConfigurationId</span></span>|<span data-ttu-id="1a2ca-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a2ca-115">String</span></span>|<span data-ttu-id="1a2ca-116">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1a2ca-116">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a2ca-117">Relações</span><span class="sxs-lookup"><span data-stu-id="1a2ca-117">Relationships</span></span>
<span data-ttu-id="1a2ca-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1a2ca-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a2ca-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a2ca-119">JSON Representation</span></span>
<span data-ttu-id="1a2ca-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a2ca-120">Here is a JSON representation of the resource.</span></span>
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



