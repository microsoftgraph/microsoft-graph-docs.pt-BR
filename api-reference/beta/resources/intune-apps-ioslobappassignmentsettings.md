---
title: Tipo de recurso iosLobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: db267df76db2171a869667e62e33d94644652ec8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882107"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="4db53-103">Tipo de recurso iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="4db53-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="4db53-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4db53-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4db53-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4db53-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4db53-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4db53-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4db53-107">Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.</span><span class="sxs-lookup"><span data-stu-id="4db53-107">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>

<span data-ttu-id="4db53-108">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="4db53-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4db53-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4db53-109">Properties</span></span>
|<span data-ttu-id="4db53-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4db53-110">Property</span></span>|<span data-ttu-id="4db53-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="4db53-111">Type</span></span>|<span data-ttu-id="4db53-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4db53-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4db53-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="4db53-113">vpnConfigurationId</span></span>|<span data-ttu-id="4db53-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4db53-114">String</span></span>|<span data-ttu-id="4db53-115">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4db53-115">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4db53-116">Relações</span><span class="sxs-lookup"><span data-stu-id="4db53-116">Relationships</span></span>
<span data-ttu-id="4db53-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4db53-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4db53-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4db53-118">JSON Representation</span></span>
<span data-ttu-id="4db53-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4db53-119">Here is a JSON representation of the resource.</span></span>
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





