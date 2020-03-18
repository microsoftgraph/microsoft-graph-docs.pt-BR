---
title: tipo de recurso windowsAppXAppAssignmentSettings
description: Contém propriedades usadas ao atribuir um aplicativo móvel do Windows AppX a um grupo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7f0732a9399f711d3db8b9e95b57182877879fc8
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42766851"
---
# <a name="windowsappxappassignmentsettings-resource-type"></a><span data-ttu-id="9ca7d-103">tipo de recurso windowsAppXAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="9ca7d-103">windowsAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="9ca7d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9ca7d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ca7d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9ca7d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ca7d-106">Contém propriedades usadas ao atribuir um aplicativo móvel do Windows AppX a um grupo.</span><span class="sxs-lookup"><span data-stu-id="9ca7d-106">Contains properties used when assigning a Windows AppX mobile app to a group.</span></span>


<span data-ttu-id="9ca7d-107">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="9ca7d-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9ca7d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9ca7d-108">Properties</span></span>
|<span data-ttu-id="9ca7d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ca7d-109">Property</span></span>|<span data-ttu-id="9ca7d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ca7d-110">Type</span></span>|<span data-ttu-id="9ca7d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ca7d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ca7d-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="9ca7d-112">useDeviceContext</span></span>|<span data-ttu-id="9ca7d-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="9ca7d-113">Boolean</span></span>|<span data-ttu-id="9ca7d-114">Se o contexto de execução de dispositivo deve ou não ser usado para o aplicativo móvel do Windows AppX.</span><span class="sxs-lookup"><span data-stu-id="9ca7d-114">Whether or not to use device execution context for Windows AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ca7d-115">Relações</span><span class="sxs-lookup"><span data-stu-id="9ca7d-115">Relationships</span></span>
<span data-ttu-id="9ca7d-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9ca7d-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ca7d-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ca7d-117">JSON Representation</span></span>
<span data-ttu-id="9ca7d-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9ca7d-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsAppXAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAppXAppAssignmentSettings",
  "useDeviceContext": true
}
```



