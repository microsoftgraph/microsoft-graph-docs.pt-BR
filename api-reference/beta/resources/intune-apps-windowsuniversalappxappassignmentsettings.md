---
title: tipo de recurso windowsUniversalAppXAppAssignmentSettings
description: Contém propriedades usadas ao atribuir um aplicativo móvel do Windows universal AppX a um grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4291a240bd5cd93e289fd916f141759f90a52d1d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004901"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a><span data-ttu-id="aeba8-103">tipo de recurso windowsUniversalAppXAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="aeba8-103">windowsUniversalAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="aeba8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aeba8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aeba8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aeba8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aeba8-106">Contém propriedades usadas ao atribuir um aplicativo móvel do Windows universal AppX a um grupo.</span><span class="sxs-lookup"><span data-stu-id="aeba8-106">Contains properties used when assigning a Windows Universal AppX mobile app to a group.</span></span>


<span data-ttu-id="aeba8-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="aeba8-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aeba8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aeba8-108">Properties</span></span>
|<span data-ttu-id="aeba8-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aeba8-109">Property</span></span>|<span data-ttu-id="aeba8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="aeba8-110">Type</span></span>|<span data-ttu-id="aeba8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="aeba8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aeba8-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="aeba8-112">useDeviceContext</span></span>|<span data-ttu-id="aeba8-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="aeba8-113">Boolean</span></span>|<span data-ttu-id="aeba8-114">Se o contexto de execução de dispositivo deve ou não ser usado para o aplicativo móvel do Windows universal AppX.</span><span class="sxs-lookup"><span data-stu-id="aeba8-114">Whether or not to use device execution context for Windows Universal AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aeba8-115">Relações</span><span class="sxs-lookup"><span data-stu-id="aeba8-115">Relationships</span></span>
<span data-ttu-id="aeba8-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aeba8-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aeba8-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aeba8-117">JSON Representation</span></span>
<span data-ttu-id="aeba8-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aeba8-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUniversalAppXAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXAppAssignmentSettings",
  "useDeviceContext": true
}
```





