---
title: Tipo de recurso iosVppAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1148336c5fa868cea90f223e66bf3868775647c6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423675"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="80bfb-103">Tipo de recurso iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="80bfb-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="80bfb-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="80bfb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="80bfb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="80bfb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80bfb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="80bfb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80bfb-107">Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="80bfb-107">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="80bfb-108">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="80bfb-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="80bfb-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80bfb-109">Properties</span></span>
|<span data-ttu-id="80bfb-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80bfb-110">Property</span></span>|<span data-ttu-id="80bfb-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="80bfb-111">Type</span></span>|<span data-ttu-id="80bfb-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="80bfb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80bfb-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="80bfb-113">useDeviceLicensing</span></span>|<span data-ttu-id="80bfb-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="80bfb-114">Boolean</span></span>|<span data-ttu-id="80bfb-115">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80bfb-115">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="80bfb-116">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="80bfb-116">vpnConfigurationId</span></span>|<span data-ttu-id="80bfb-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80bfb-117">String</span></span>|<span data-ttu-id="80bfb-118">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="80bfb-118">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80bfb-119">Relações</span><span class="sxs-lookup"><span data-stu-id="80bfb-119">Relationships</span></span>
<span data-ttu-id="80bfb-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="80bfb-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="80bfb-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80bfb-121">JSON Representation</span></span>
<span data-ttu-id="80bfb-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="80bfb-122">Here is a JSON representation of the resource.</span></span>
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




