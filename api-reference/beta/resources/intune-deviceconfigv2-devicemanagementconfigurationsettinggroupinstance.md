---
title: tipo de recurso deviceManagementConfigurationSettingGroupInstance
description: Configuração de instância dentro da política
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1ab5093675e8d1bc9b0796a5a937b9bed894ca24
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241138"
---
# <a name="devicemanagementconfigurationsettinggroupinstance-resource-type"></a><span data-ttu-id="ed654-103">tipo de recurso deviceManagementConfigurationSettingGroupInstance</span><span class="sxs-lookup"><span data-stu-id="ed654-103">deviceManagementConfigurationSettingGroupInstance resource type</span></span>

<span data-ttu-id="ed654-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed654-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed654-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ed654-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed654-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ed654-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed654-107">Configuração de instância dentro da política</span><span class="sxs-lookup"><span data-stu-id="ed654-107">Setting instance within policy</span></span>


<span data-ttu-id="ed654-108">Herda de [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="ed654-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ed654-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed654-109">Properties</span></span>
|<span data-ttu-id="ed654-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed654-110">Property</span></span>|<span data-ttu-id="ed654-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed654-111">Type</span></span>|<span data-ttu-id="ed654-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed654-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed654-113">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="ed654-113">settingDefinitionId</span></span>|<span data-ttu-id="ed654-114">String</span><span class="sxs-lookup"><span data-stu-id="ed654-114">String</span></span>|<span data-ttu-id="ed654-115">Definição de ID de definição herdada de [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="ed654-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed654-116">Relações</span><span class="sxs-lookup"><span data-stu-id="ed654-116">Relationships</span></span>
<span data-ttu-id="ed654-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ed654-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed654-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed654-118">JSON Representation</span></span>
<span data-ttu-id="ed654-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed654-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingGroupInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupInstance",
  "settingDefinitionId": "String"
}
```




