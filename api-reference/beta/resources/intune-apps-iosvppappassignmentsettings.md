---
title: Tipo de recurso iosVppAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.
ms.openlocfilehash: c7ae6221aa978cc1412de25521dd8b08ff72c0c3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038719"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="cdf0b-103">Tipo de recurso iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="cdf0b-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="cdf0b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cdf0b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cdf0b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cdf0b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cdf0b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cdf0b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cdf0b-107">Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="cdf0b-107">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="cdf0b-108">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="cdf0b-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cdf0b-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cdf0b-109">Properties</span></span>
|<span data-ttu-id="cdf0b-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cdf0b-110">Property</span></span>|<span data-ttu-id="cdf0b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="cdf0b-111">Type</span></span>|<span data-ttu-id="cdf0b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdf0b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdf0b-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="cdf0b-113">useDeviceLicensing</span></span>|<span data-ttu-id="cdf0b-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="cdf0b-114">Boolean</span></span>|<span data-ttu-id="cdf0b-115">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cdf0b-115">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="cdf0b-116">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="cdf0b-116">vpnConfigurationId</span></span>|<span data-ttu-id="cdf0b-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cdf0b-117">String</span></span>|<span data-ttu-id="cdf0b-118">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="cdf0b-118">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cdf0b-119">Relações</span><span class="sxs-lookup"><span data-stu-id="cdf0b-119">Relationships</span></span>
<span data-ttu-id="cdf0b-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cdf0b-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cdf0b-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cdf0b-121">JSON Representation</span></span>
<span data-ttu-id="cdf0b-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cdf0b-122">Here is a JSON representation of the resource.</span></span>
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





