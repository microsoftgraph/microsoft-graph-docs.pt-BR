---
title: tipo de recurso officeConfigurationGroupAssignmentTarget
description: Destino de atribuição de grupo AAD de configuração de cliente do Office.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7a3451d4bddec96c1e21cd605b05cb34d96372ff
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153547"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="d3d58-103">tipo de recurso officeConfigurationGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d3d58-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="d3d58-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d3d58-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3d58-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d3d58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3d58-106">Destino de atribuição de grupo AAD de configuração de cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="d3d58-106">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="d3d58-107">Herda de [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="d3d58-107">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d3d58-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d3d58-108">Properties</span></span>
|<span data-ttu-id="d3d58-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3d58-109">Property</span></span>|<span data-ttu-id="d3d58-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3d58-110">Type</span></span>|<span data-ttu-id="d3d58-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3d58-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3d58-112">groupId</span><span class="sxs-lookup"><span data-stu-id="d3d58-112">groupId</span></span>|<span data-ttu-id="d3d58-113">String</span><span class="sxs-lookup"><span data-stu-id="d3d58-113">String</span></span>|<span data-ttu-id="d3d58-114">A ID do grupo do AAD no qual estamos direcionando a configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d3d58-114">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3d58-115">Relações</span><span class="sxs-lookup"><span data-stu-id="d3d58-115">Relationships</span></span>
<span data-ttu-id="d3d58-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d3d58-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3d58-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d3d58-117">JSON Representation</span></span>
<span data-ttu-id="d3d58-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d3d58-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfigurationGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfigurationGroupAssignmentTarget",
  "groupId": "String"
}
```



