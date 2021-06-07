---
title: Tipo de recurso iosStoreAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS Store para um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0b47c71f151e0cb83f9e682789fcde3a7b69ae4b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756068"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="22e29-103">Tipo de recurso iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="22e29-103">iosStoreAppAssignmentSettings resource type</span></span>

<span data-ttu-id="22e29-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22e29-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22e29-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="22e29-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22e29-106">Contém propriedades usadas para atribuir um aplicativo móvel da iOS Store para um grupo.</span><span class="sxs-lookup"><span data-stu-id="22e29-106">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="22e29-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="22e29-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="22e29-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="22e29-108">Properties</span></span>
|<span data-ttu-id="22e29-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22e29-109">Property</span></span>|<span data-ttu-id="22e29-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="22e29-110">Type</span></span>|<span data-ttu-id="22e29-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="22e29-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22e29-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="22e29-112">vpnConfigurationId</span></span>|<span data-ttu-id="22e29-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="22e29-113">String</span></span>|<span data-ttu-id="22e29-114">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="22e29-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22e29-115">Relações</span><span class="sxs-lookup"><span data-stu-id="22e29-115">Relationships</span></span>
<span data-ttu-id="22e29-116">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="22e29-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="22e29-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="22e29-117">JSON Representation</span></span>
<span data-ttu-id="22e29-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="22e29-118">Here is a JSON representation of the resource.</span></span>
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




