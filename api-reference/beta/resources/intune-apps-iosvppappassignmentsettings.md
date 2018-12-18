---
title: Tipo de recurso iosVppAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.
author: tfitzmac
ms.openlocfilehash: 9e1233c9d5a33876da64ab3c75419c322ee83931
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321326"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="79ef5-103">Tipo de recurso iosVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="79ef5-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="79ef5-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="79ef5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79ef5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="79ef5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="79ef5-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="79ef5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="79ef5-107">Contém propriedades usadas para atribuir um aplicativo móvel do iOS VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="79ef5-107">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="79ef5-108">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="79ef5-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="79ef5-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79ef5-109">Properties</span></span>
|<span data-ttu-id="79ef5-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79ef5-110">Property</span></span>|<span data-ttu-id="79ef5-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="79ef5-111">Type</span></span>|<span data-ttu-id="79ef5-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="79ef5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79ef5-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="79ef5-113">useDeviceLicensing</span></span>|<span data-ttu-id="79ef5-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="79ef5-114">Boolean</span></span>|<span data-ttu-id="79ef5-115">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="79ef5-115">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="79ef5-116">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="79ef5-116">vpnConfigurationId</span></span>|<span data-ttu-id="79ef5-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="79ef5-117">String</span></span>|<span data-ttu-id="79ef5-118">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="79ef5-118">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79ef5-119">Relações</span><span class="sxs-lookup"><span data-stu-id="79ef5-119">Relationships</span></span>
<span data-ttu-id="79ef5-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="79ef5-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="79ef5-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79ef5-121">JSON Representation</span></span>
<span data-ttu-id="79ef5-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="79ef5-122">Here is a JSON representation of the resource.</span></span>
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





