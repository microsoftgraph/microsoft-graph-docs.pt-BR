---
title: Tipo de recurso iosStoreAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel da iOS Store para um grupo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b83422a937bf9a067bd55c4ef09806e01bc51ad9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474317"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="bc0f4-103">Tipo de recurso iosStoreAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="bc0f4-103">iosStoreAppAssignmentSettings resource type</span></span>

<span data-ttu-id="bc0f4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc0f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc0f4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bc0f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc0f4-106">Contém propriedades usadas para atribuir um aplicativo móvel da iOS Store para um grupo.</span><span class="sxs-lookup"><span data-stu-id="bc0f4-106">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="bc0f4-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="bc0f4-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bc0f4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bc0f4-108">Properties</span></span>
|<span data-ttu-id="bc0f4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc0f4-109">Property</span></span>|<span data-ttu-id="bc0f4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc0f4-110">Type</span></span>|<span data-ttu-id="bc0f4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc0f4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc0f4-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="bc0f4-112">vpnConfigurationId</span></span>|<span data-ttu-id="bc0f4-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc0f4-113">String</span></span>|<span data-ttu-id="bc0f4-114">A identificação de configuração da VPN a aplicar neste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bc0f4-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc0f4-115">Relações</span><span class="sxs-lookup"><span data-stu-id="bc0f4-115">Relationships</span></span>
<span data-ttu-id="bc0f4-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bc0f4-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc0f4-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bc0f4-117">JSON Representation</span></span>
<span data-ttu-id="bc0f4-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bc0f4-118">Here is a JSON representation of the resource.</span></span>
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







