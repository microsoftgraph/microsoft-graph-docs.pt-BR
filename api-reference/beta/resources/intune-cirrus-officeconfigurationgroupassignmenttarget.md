---
title: tipo de recurso officeConfigurationGroupAssignmentTarget
description: Destino de atribuição de grupo AAD de configuração de cliente do Office.
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9e09d73695c542c24fe6be297dec9496794d95fc
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43454280"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="8e197-103">tipo de recurso officeConfigurationGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8e197-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="8e197-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e197-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e197-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8e197-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e197-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8e197-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e197-107">Destino de atribuição de grupo AAD de configuração de cliente do Office.</span><span class="sxs-lookup"><span data-stu-id="8e197-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="8e197-108">Herda de [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="8e197-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8e197-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8e197-109">Properties</span></span>
|<span data-ttu-id="8e197-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8e197-110">Property</span></span>|<span data-ttu-id="8e197-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="8e197-111">Type</span></span>|<span data-ttu-id="8e197-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e197-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e197-113">groupId</span><span class="sxs-lookup"><span data-stu-id="8e197-113">groupId</span></span>|<span data-ttu-id="8e197-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8e197-114">String</span></span>|<span data-ttu-id="8e197-115">A ID do grupo do AAD no qual estamos direcionando a configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8e197-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e197-116">Relações</span><span class="sxs-lookup"><span data-stu-id="8e197-116">Relationships</span></span>
<span data-ttu-id="8e197-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8e197-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e197-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8e197-118">JSON Representation</span></span>
<span data-ttu-id="8e197-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8e197-119">Here is a JSON representation of the resource.</span></span>
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



