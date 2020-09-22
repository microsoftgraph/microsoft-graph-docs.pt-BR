---
title: tipo de recurso macOsVppAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel do Mac VPP a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4fde5787e77827950bab4b5f68bf94325eea3446
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095090"
---
# <a name="macosvppappassignmentsettings-resource-type"></a><span data-ttu-id="7ec81-103">tipo de recurso macOsVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="7ec81-103">macOsVppAppAssignmentSettings resource type</span></span>

<span data-ttu-id="7ec81-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ec81-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ec81-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7ec81-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ec81-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7ec81-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ec81-107">Contém propriedades usadas para atribuir um aplicativo móvel do Mac VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="7ec81-107">Contains properties used to assign an Mac VPP mobile app to a group.</span></span>


<span data-ttu-id="7ec81-108">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="7ec81-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7ec81-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ec81-109">Properties</span></span>
|<span data-ttu-id="7ec81-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ec81-110">Property</span></span>|<span data-ttu-id="7ec81-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ec81-111">Type</span></span>|<span data-ttu-id="7ec81-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ec81-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ec81-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="7ec81-113">useDeviceLicensing</span></span>|<span data-ttu-id="7ec81-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="7ec81-114">Boolean</span></span>|<span data-ttu-id="7ec81-115">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7ec81-115">Whether or not to use device licensing.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ec81-116">Relações</span><span class="sxs-lookup"><span data-stu-id="7ec81-116">Relationships</span></span>
<span data-ttu-id="7ec81-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7ec81-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ec81-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ec81-118">JSON Representation</span></span>
<span data-ttu-id="7ec81-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7ec81-119">Here is a JSON representation of the resource.</span></span>
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






