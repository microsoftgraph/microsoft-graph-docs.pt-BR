---
title: Tipo de recurso iosStoreAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS Store para um grupo.
author: tfitzmac
ms.openlocfilehash: 19a9ba760a0e375d6afa4c504fd57e6ecac4d2ce
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303945"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="4a7b8-103">Tipo de recurso iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="4a7b8-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="4a7b8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4a7b8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a7b8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4a7b8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4a7b8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4a7b8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a7b8-107">Contém propriedades usadas para atribuir um aplicativo móvel da iOS Store para um grupo.</span><span class="sxs-lookup"><span data-stu-id="4a7b8-107">Contains properties used to assign an iOS Store mobile app to a group.</span></span>

<span data-ttu-id="4a7b8-108">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="4a7b8-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4a7b8-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a7b8-109">Properties</span></span>
|<span data-ttu-id="4a7b8-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a7b8-110">Property</span></span>|<span data-ttu-id="4a7b8-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a7b8-111">Type</span></span>|<span data-ttu-id="4a7b8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a7b8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a7b8-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="4a7b8-113">vpnConfigurationId</span></span>|<span data-ttu-id="4a7b8-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a7b8-114">String</span></span>|<span data-ttu-id="4a7b8-115">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4a7b8-115">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a7b8-116">Relações</span><span class="sxs-lookup"><span data-stu-id="4a7b8-116">Relationships</span></span>
<span data-ttu-id="4a7b8-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4a7b8-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4a7b8-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a7b8-118">JSON Representation</span></span>
<span data-ttu-id="4a7b8-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4a7b8-119">Here is a JSON representation of the resource.</span></span>
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





