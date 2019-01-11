---
title: Tipo de recurso iosVppAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2dd3f8816aaa4e08066e329e4a9f4630e3f27f1d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867764"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="b0442-103">Tipo de recurso iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="b0442-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="b0442-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b0442-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0442-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b0442-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b0442-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b0442-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0442-107">Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="b0442-107">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="b0442-108">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="b0442-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b0442-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0442-109">Properties</span></span>
|<span data-ttu-id="b0442-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0442-110">Property</span></span>|<span data-ttu-id="b0442-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0442-111">Type</span></span>|<span data-ttu-id="b0442-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0442-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0442-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="b0442-113">useDeviceLicensing</span></span>|<span data-ttu-id="b0442-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="b0442-114">Boolean</span></span>|<span data-ttu-id="b0442-115">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b0442-115">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="b0442-116">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="b0442-116">vpnConfigurationId</span></span>|<span data-ttu-id="b0442-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0442-117">String</span></span>|<span data-ttu-id="b0442-118">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b0442-118">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0442-119">Relações</span><span class="sxs-lookup"><span data-stu-id="b0442-119">Relationships</span></span>
<span data-ttu-id="b0442-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b0442-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b0442-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0442-121">JSON Representation</span></span>
<span data-ttu-id="b0442-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0442-122">Here is a JSON representation of the resource.</span></span>
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





