---
title: tipo de recurso windowsAppXAppAssignmentSettings
description: Contém propriedades usadas ao atribuir um aplicativo móvel do Windows AppX a um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f15af8bf60dae2b40473eb23a1093f9e73bda7b6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785920"
---
# <a name="windowsappxappassignmentsettings-resource-type"></a><span data-ttu-id="75a2b-103">tipo de recurso windowsAppXAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="75a2b-103">windowsAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="75a2b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="75a2b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75a2b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75a2b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75a2b-106">Contém propriedades usadas ao atribuir um aplicativo móvel do Windows AppX a um grupo.</span><span class="sxs-lookup"><span data-stu-id="75a2b-106">Contains properties used when assigning a Windows AppX mobile app to a group.</span></span>


<span data-ttu-id="75a2b-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="75a2b-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="75a2b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="75a2b-108">Properties</span></span>
|<span data-ttu-id="75a2b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75a2b-109">Property</span></span>|<span data-ttu-id="75a2b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="75a2b-110">Type</span></span>|<span data-ttu-id="75a2b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="75a2b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75a2b-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="75a2b-112">useDeviceContext</span></span>|<span data-ttu-id="75a2b-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="75a2b-113">Boolean</span></span>|<span data-ttu-id="75a2b-114">Se o contexto de execução de dispositivo deve ou não ser usado para o aplicativo móvel do Windows AppX.</span><span class="sxs-lookup"><span data-stu-id="75a2b-114">Whether or not to use device execution context for Windows AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75a2b-115">Relações</span><span class="sxs-lookup"><span data-stu-id="75a2b-115">Relationships</span></span>
<span data-ttu-id="75a2b-116">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="75a2b-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="75a2b-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75a2b-117">JSON Representation</span></span>
<span data-ttu-id="75a2b-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="75a2b-118">Here is a JSON representation of the resource.</span></span>
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





