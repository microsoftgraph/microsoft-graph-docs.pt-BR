---
title: tipo de recurso windowsUniversalAppXAppAssignmentSettings
description: Contém propriedades usadas ao atribuir um aplicativo móvel do Windows universal AppX a um grupo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dc945c303d49a97aeb45bf72e4fb8b5ffb7ab377
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447968"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a><span data-ttu-id="ff4e2-103">tipo de recurso windowsUniversalAppXAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="ff4e2-103">windowsUniversalAppXAppAssignmentSettings resource type</span></span>

<span data-ttu-id="ff4e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff4e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff4e2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ff4e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff4e2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ff4e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff4e2-107">Contém propriedades usadas ao atribuir um aplicativo móvel do Windows universal AppX a um grupo.</span><span class="sxs-lookup"><span data-stu-id="ff4e2-107">Contains properties used when assigning a Windows Universal AppX mobile app to a group.</span></span>


<span data-ttu-id="ff4e2-108">Herda de [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="ff4e2-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ff4e2-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff4e2-109">Properties</span></span>
|<span data-ttu-id="ff4e2-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff4e2-110">Property</span></span>|<span data-ttu-id="ff4e2-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff4e2-111">Type</span></span>|<span data-ttu-id="ff4e2-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff4e2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff4e2-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="ff4e2-113">useDeviceContext</span></span>|<span data-ttu-id="ff4e2-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="ff4e2-114">Boolean</span></span>|<span data-ttu-id="ff4e2-115">Se o contexto de execução de dispositivo deve ou não ser usado para o aplicativo móvel do Windows universal AppX.</span><span class="sxs-lookup"><span data-stu-id="ff4e2-115">Whether or not to use device execution context for Windows Universal AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff4e2-116">Relações</span><span class="sxs-lookup"><span data-stu-id="ff4e2-116">Relationships</span></span>
<span data-ttu-id="ff4e2-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ff4e2-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff4e2-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff4e2-118">JSON Representation</span></span>
<span data-ttu-id="ff4e2-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff4e2-119">Here is a JSON representation of the resource.</span></span>
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



