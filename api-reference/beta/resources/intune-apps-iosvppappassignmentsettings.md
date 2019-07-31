---
title: Tipo de recurso iosVppAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 77480c88e6fd210704a47f60293081b1ede2e6ca
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005924"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="29911-103">Tipo de recurso iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="29911-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="29911-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="29911-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29911-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="29911-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29911-106">Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="29911-106">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="29911-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="29911-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="29911-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="29911-108">Properties</span></span>
|<span data-ttu-id="29911-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29911-109">Property</span></span>|<span data-ttu-id="29911-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="29911-110">Type</span></span>|<span data-ttu-id="29911-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="29911-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29911-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="29911-112">useDeviceLicensing</span></span>|<span data-ttu-id="29911-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="29911-113">Boolean</span></span>|<span data-ttu-id="29911-114">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="29911-114">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="29911-115">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="29911-115">vpnConfigurationId</span></span>|<span data-ttu-id="29911-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29911-116">String</span></span>|<span data-ttu-id="29911-117">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="29911-117">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29911-118">Relações</span><span class="sxs-lookup"><span data-stu-id="29911-118">Relationships</span></span>
<span data-ttu-id="29911-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="29911-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="29911-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="29911-120">JSON Representation</span></span>
<span data-ttu-id="29911-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="29911-121">Here is a JSON representation of the resource.</span></span>
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





