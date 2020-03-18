---
title: tipo de recurso macOsVppAppAssignmentSettings
description: Contém propriedades usadas para atribuir um aplicativo móvel do Mac VPP a um grupo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d1b4ecb5f2dbbca6d3f9fe8eebc3771347739e77
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42769063"
---
# <a name="macosvppappassignmentsettings-resource-type"></a><span data-ttu-id="1c085-103">tipo de recurso macOsVppAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="1c085-103">macOsVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="1c085-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1c085-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c085-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1c085-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c085-106">Contém propriedades usadas para atribuir um aplicativo móvel do Mac VPP a um grupo.</span><span class="sxs-lookup"><span data-stu-id="1c085-106">Contains properties used to assign an Mac VPP mobile app to a group.</span></span>


<span data-ttu-id="1c085-107">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="1c085-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1c085-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1c085-108">Properties</span></span>
|<span data-ttu-id="1c085-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1c085-109">Property</span></span>|<span data-ttu-id="1c085-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1c085-110">Type</span></span>|<span data-ttu-id="1c085-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1c085-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c085-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="1c085-112">useDeviceLicensing</span></span>|<span data-ttu-id="1c085-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="1c085-113">Boolean</span></span>|<span data-ttu-id="1c085-114">Se usa ou não o licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1c085-114">Whether or not to use device licensing.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c085-115">Relações</span><span class="sxs-lookup"><span data-stu-id="1c085-115">Relationships</span></span>
<span data-ttu-id="1c085-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1c085-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c085-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1c085-117">JSON Representation</span></span>
<span data-ttu-id="1c085-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1c085-118">Here is a JSON representation of the resource.</span></span>
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



