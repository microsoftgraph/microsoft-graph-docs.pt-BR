---
title: Tipo de recurso officeConfigurationGroupAssignmentTarget
description: Office de configuração do cliente Destino de atribuição de grupo AAD.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6d951db7a71474cc405f4b7f97419f1a06dd502d
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666800"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="b0bd7-103">Tipo de recurso officeConfigurationGroupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b0bd7-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

<span data-ttu-id="b0bd7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0bd7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0bd7-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b0bd7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0bd7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0bd7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0bd7-107">Office de configuração do cliente Destino de atribuição de grupo AAD.</span><span class="sxs-lookup"><span data-stu-id="b0bd7-107">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="b0bd7-108">Herda de [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="b0bd7-108">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b0bd7-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0bd7-109">Properties</span></span>
|<span data-ttu-id="b0bd7-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0bd7-110">Property</span></span>|<span data-ttu-id="b0bd7-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0bd7-111">Type</span></span>|<span data-ttu-id="b0bd7-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0bd7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0bd7-113">groupId</span><span class="sxs-lookup"><span data-stu-id="b0bd7-113">groupId</span></span>|<span data-ttu-id="b0bd7-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0bd7-114">String</span></span>|<span data-ttu-id="b0bd7-115">A ID do grupo AAD para o que estamos direcionando a configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b0bd7-115">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0bd7-116">Relações</span><span class="sxs-lookup"><span data-stu-id="b0bd7-116">Relationships</span></span>
<span data-ttu-id="b0bd7-117">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="b0bd7-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0bd7-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0bd7-118">JSON Representation</span></span>
<span data-ttu-id="b0bd7-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0bd7-119">Here is a JSON representation of the resource.</span></span>
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




