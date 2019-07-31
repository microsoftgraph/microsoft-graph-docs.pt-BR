---
title: Tipo de recurso iosStoreAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS Store para um grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: afd310f3b49d7d0dfa2d5f2bbcbb836c09ab2bf2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005503"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="d3129-103">Tipo de recurso iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="d3129-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="d3129-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d3129-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3129-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d3129-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3129-106">Contém propriedades usadas para atribuir um aplicativo móvel da iOS Store para um grupo.</span><span class="sxs-lookup"><span data-stu-id="d3129-106">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="d3129-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="d3129-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d3129-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d3129-108">Properties</span></span>
|<span data-ttu-id="d3129-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3129-109">Property</span></span>|<span data-ttu-id="d3129-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3129-110">Type</span></span>|<span data-ttu-id="d3129-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3129-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3129-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="d3129-112">vpnConfigurationId</span></span>|<span data-ttu-id="d3129-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d3129-113">String</span></span>|<span data-ttu-id="d3129-114">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d3129-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3129-115">Relações</span><span class="sxs-lookup"><span data-stu-id="d3129-115">Relationships</span></span>
<span data-ttu-id="d3129-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d3129-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3129-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d3129-117">JSON Representation</span></span>
<span data-ttu-id="d3129-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d3129-118">Here is a JSON representation of the resource.</span></span>
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





