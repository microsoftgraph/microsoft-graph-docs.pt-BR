---
title: tipo de recurso windowsAppXAppAssignmentSettings
description: Contém propriedades usadas ao atribuir um aplicativo móvel do Windows AppX a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 04dd288d24f46282245ba5352b3e0792a7081c0b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089473"
---
# <a name="windowsappxappassignmentsettings-resource-type"></a><span data-ttu-id="09eb6-103">tipo de recurso windowsAppXAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="09eb6-103">windowsAppXAppAssignmentSettings resource type</span></span>

<span data-ttu-id="09eb6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09eb6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09eb6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="09eb6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09eb6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="09eb6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09eb6-107">Contém propriedades usadas ao atribuir um aplicativo móvel do Windows AppX a um grupo.</span><span class="sxs-lookup"><span data-stu-id="09eb6-107">Contains properties used when assigning a Windows AppX mobile app to a group.</span></span>


<span data-ttu-id="09eb6-108">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="09eb6-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="09eb6-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="09eb6-109">Properties</span></span>
|<span data-ttu-id="09eb6-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09eb6-110">Property</span></span>|<span data-ttu-id="09eb6-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="09eb6-111">Type</span></span>|<span data-ttu-id="09eb6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="09eb6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09eb6-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="09eb6-113">useDeviceContext</span></span>|<span data-ttu-id="09eb6-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="09eb6-114">Boolean</span></span>|<span data-ttu-id="09eb6-115">Se o contexto de execução de dispositivo deve ou não ser usado para o aplicativo móvel do Windows AppX.</span><span class="sxs-lookup"><span data-stu-id="09eb6-115">Whether or not to use device execution context for Windows AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09eb6-116">Relações</span><span class="sxs-lookup"><span data-stu-id="09eb6-116">Relationships</span></span>
<span data-ttu-id="09eb6-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="09eb6-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09eb6-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="09eb6-118">JSON Representation</span></span>
<span data-ttu-id="09eb6-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="09eb6-119">Here is a JSON representation of the resource.</span></span>
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






