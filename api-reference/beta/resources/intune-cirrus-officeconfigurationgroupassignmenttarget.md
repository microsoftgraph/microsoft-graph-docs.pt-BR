---
title: tipo de recurso officeConfigurationGroupAssignmentTarget
description: Destino de atribuição de grupo AAD de configuração de cliente do Office.
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: 7458b1071b6133f3b46c8412270e30fdd0bf7638
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949308"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="4fb7a-103">tipo de recurso officeConfigurationGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4fb7a-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="4fb7a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4fb7a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fb7a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4fb7a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fb7a-106">Destino de atribuição de grupo AAD de configuração de cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="4fb7a-106">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="4fb7a-107">Herda de [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="4fb7a-107">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4fb7a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4fb7a-108">Properties</span></span>
|<span data-ttu-id="4fb7a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4fb7a-109">Property</span></span>|<span data-ttu-id="4fb7a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4fb7a-110">Type</span></span>|<span data-ttu-id="4fb7a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4fb7a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fb7a-112">groupId</span><span class="sxs-lookup"><span data-stu-id="4fb7a-112">groupId</span></span>|<span data-ttu-id="4fb7a-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4fb7a-113">String</span></span>|<span data-ttu-id="4fb7a-114">A ID do grupo do AAD no qual estamos direcionando a configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4fb7a-114">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4fb7a-115">Relações</span><span class="sxs-lookup"><span data-stu-id="4fb7a-115">Relationships</span></span>
<span data-ttu-id="4fb7a-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4fb7a-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4fb7a-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4fb7a-117">JSON Representation</span></span>
<span data-ttu-id="4fb7a-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4fb7a-118">Here is a JSON representation of the resource.</span></span>
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



