---
title: tipo de recurso windowsUniversalAppXAppAssignmentSettings
description: Contém propriedades usadas ao atribuir um aplicativo móvel do Windows universal AppX a um grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e8928634dd9e169b0550e10ec4d43ac638519bfa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523454"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a><span data-ttu-id="bd228-103">tipo de recurso windowsUniversalAppXAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="bd228-103">windowsUniversalAppXAppAssignmentSettings resource type</span></span>

<span data-ttu-id="bd228-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd228-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bd228-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bd228-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd228-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bd228-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd228-107">Contém propriedades usadas ao atribuir um aplicativo móvel do Windows universal AppX a um grupo.</span><span class="sxs-lookup"><span data-stu-id="bd228-107">Contains properties used when assigning a Windows Universal AppX mobile app to a group.</span></span>


<span data-ttu-id="bd228-108">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="bd228-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bd228-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bd228-109">Properties</span></span>
|<span data-ttu-id="bd228-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bd228-110">Property</span></span>|<span data-ttu-id="bd228-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd228-111">Type</span></span>|<span data-ttu-id="bd228-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd228-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd228-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="bd228-113">useDeviceContext</span></span>|<span data-ttu-id="bd228-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="bd228-114">Boolean</span></span>|<span data-ttu-id="bd228-115">Se o contexto de execução de dispositivo deve ou não ser usado para o aplicativo móvel do Windows universal AppX.</span><span class="sxs-lookup"><span data-stu-id="bd228-115">Whether or not to use device execution context for Windows Universal AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd228-116">Relações</span><span class="sxs-lookup"><span data-stu-id="bd228-116">Relationships</span></span>
<span data-ttu-id="bd228-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bd228-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd228-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bd228-118">JSON Representation</span></span>
<span data-ttu-id="bd228-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bd228-119">Here is a JSON representation of the resource.</span></span>
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



