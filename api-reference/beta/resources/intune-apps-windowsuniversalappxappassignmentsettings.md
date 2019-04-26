---
title: tipo de recurso windowsUniversalAppXAppAssignmentSettings
description: Contém propriedades usadas ao atribuir um aplicativo móvel do Windows universal AppX a um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eeb724c9701b9bf0e82aa4d77689e8c2f58fe552
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558381"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a><span data-ttu-id="a0c49-103">tipo de recurso windowsUniversalAppXAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="a0c49-103">windowsUniversalAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="a0c49-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a0c49-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0c49-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a0c49-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0c49-106">Contém propriedades usadas ao atribuir um aplicativo móvel do Windows universal AppX a um grupo.</span><span class="sxs-lookup"><span data-stu-id="a0c49-106">Contains properties used when assigning a Windows Universal AppX mobile app to a group.</span></span>


<span data-ttu-id="a0c49-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="a0c49-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a0c49-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0c49-108">Properties</span></span>
|<span data-ttu-id="a0c49-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0c49-109">Property</span></span>|<span data-ttu-id="a0c49-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0c49-110">Type</span></span>|<span data-ttu-id="a0c49-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0c49-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0c49-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="a0c49-112">useDeviceContext</span></span>|<span data-ttu-id="a0c49-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="a0c49-113">Boolean</span></span>|<span data-ttu-id="a0c49-114">Se o contexto de execução de dispositivo deve ou não ser usado para o aplicativo móvel do Windows universal AppX.</span><span class="sxs-lookup"><span data-stu-id="a0c49-114">Whether or not to use device execution context for Windows Universal AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0c49-115">Relações</span><span class="sxs-lookup"><span data-stu-id="a0c49-115">Relationships</span></span>
<span data-ttu-id="a0c49-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a0c49-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0c49-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0c49-117">JSON Representation</span></span>
<span data-ttu-id="a0c49-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a0c49-118">Here is a JSON representation of the resource.</span></span>
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





