---
title: tipo de recurso macOsVppAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel do Mac VPP a um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b55e203e58197d4b3e29d4a6a8567769d9196e0c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803224"
---
# <a name="macosvppappassignmentsettings-resource-type"></a><span data-ttu-id="7f9aa-103">tipo de recurso macOsVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="7f9aa-103">macOsVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="7f9aa-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7f9aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f9aa-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7f9aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f9aa-106">Contém propriedades usadas para atribuir um aplicativo móvel do Mac VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="7f9aa-106">Contains properties used to assign an Mac VPP mobile app to a group.</span></span>


<span data-ttu-id="7f9aa-107">Herda de [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="7f9aa-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7f9aa-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7f9aa-108">Properties</span></span>
|<span data-ttu-id="7f9aa-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f9aa-109">Property</span></span>|<span data-ttu-id="7f9aa-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f9aa-110">Type</span></span>|<span data-ttu-id="7f9aa-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f9aa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f9aa-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="7f9aa-112">useDeviceLicensing</span></span>|<span data-ttu-id="7f9aa-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="7f9aa-113">Boolean</span></span>|<span data-ttu-id="7f9aa-114">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7f9aa-114">Whether or not to use device licensing.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f9aa-115">Relações</span><span class="sxs-lookup"><span data-stu-id="7f9aa-115">Relationships</span></span>
<span data-ttu-id="7f9aa-116">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="7f9aa-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f9aa-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f9aa-117">JSON Representation</span></span>
<span data-ttu-id="7f9aa-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7f9aa-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignmentSettings",
  "useDeviceLicensing": true
}
```





