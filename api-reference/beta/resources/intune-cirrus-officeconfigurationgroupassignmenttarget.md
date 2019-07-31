---
title: tipo de recurso officeConfigurationGroupAssignmentTarget
description: Destino de atribuição de grupo AAD de configuração de cliente do Office.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fb97541a86e820e02e56a20568d3869a047dc2c3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011957"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="662df-103">tipo de recurso officeConfigurationGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="662df-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="662df-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="662df-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="662df-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="662df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="662df-106">Destino de atribuição de grupo AAD de configuração de cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="662df-106">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="662df-107">Herda de [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="662df-107">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="662df-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="662df-108">Properties</span></span>
|<span data-ttu-id="662df-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="662df-109">Property</span></span>|<span data-ttu-id="662df-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="662df-110">Type</span></span>|<span data-ttu-id="662df-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="662df-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="662df-112">groupId</span><span class="sxs-lookup"><span data-stu-id="662df-112">groupId</span></span>|<span data-ttu-id="662df-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="662df-113">String</span></span>|<span data-ttu-id="662df-114">A ID do grupo do AAD no qual estamos direcionando a configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="662df-114">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="662df-115">Relações</span><span class="sxs-lookup"><span data-stu-id="662df-115">Relationships</span></span>
<span data-ttu-id="662df-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="662df-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="662df-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="662df-117">JSON Representation</span></span>
<span data-ttu-id="662df-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="662df-118">Here is a JSON representation of the resource.</span></span>
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



