---
title: Tipo de recurso iosLobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7f2e0c9ca5b2628343b79ff972e50c3684651c23
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990506"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="07162-103">Tipo de recurso iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="07162-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="07162-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="07162-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07162-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="07162-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07162-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="07162-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="07162-107">Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.</span><span class="sxs-lookup"><span data-stu-id="07162-107">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>

<span data-ttu-id="07162-108">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="07162-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="07162-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07162-109">Properties</span></span>
|<span data-ttu-id="07162-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07162-110">Property</span></span>|<span data-ttu-id="07162-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="07162-111">Type</span></span>|<span data-ttu-id="07162-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="07162-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07162-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="07162-113">vpnConfigurationId</span></span>|<span data-ttu-id="07162-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07162-114">String</span></span>|<span data-ttu-id="07162-115">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="07162-115">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07162-116">Relações</span><span class="sxs-lookup"><span data-stu-id="07162-116">Relationships</span></span>
<span data-ttu-id="07162-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="07162-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="07162-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07162-118">JSON Representation</span></span>
<span data-ttu-id="07162-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="07162-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```





