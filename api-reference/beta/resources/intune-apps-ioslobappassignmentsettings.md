---
title: Tipo de recurso iosLobAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4f2d954b016ed2a59938974f995d9bd040bc69b1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404348"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="57867-103">Tipo de recurso iosLobAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="57867-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="57867-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="57867-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="57867-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="57867-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="57867-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="57867-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57867-107">Contém propriedades usadas para atribuir um aplicativo móvel da iOS LOB a um grupo.</span><span class="sxs-lookup"><span data-stu-id="57867-107">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="57867-108">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="57867-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="57867-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="57867-109">Properties</span></span>
|<span data-ttu-id="57867-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57867-110">Property</span></span>|<span data-ttu-id="57867-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="57867-111">Type</span></span>|<span data-ttu-id="57867-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="57867-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57867-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="57867-113">vpnConfigurationId</span></span>|<span data-ttu-id="57867-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57867-114">String</span></span>|<span data-ttu-id="57867-115">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="57867-115">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57867-116">Relações</span><span class="sxs-lookup"><span data-stu-id="57867-116">Relationships</span></span>
<span data-ttu-id="57867-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="57867-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57867-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="57867-118">JSON Representation</span></span>
<span data-ttu-id="57867-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="57867-119">Here is a JSON representation of the resource.</span></span>
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




