---
title: Tipo de recurso deviceManagementConfigurationSettingGroupCollectionInstance
description: Definindo instância dentro da política
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: af7bab6d165780c66a7f61ce0143be98bd0195b7
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665613"
---
# <a name="devicemanagementconfigurationsettinggroupcollectioninstance-resource-type"></a><span data-ttu-id="84c45-103">Tipo de recurso deviceManagementConfigurationSettingGroupCollectionInstance</span><span class="sxs-lookup"><span data-stu-id="84c45-103">deviceManagementConfigurationSettingGroupCollectionInstance resource type</span></span>

<span data-ttu-id="84c45-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84c45-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84c45-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="84c45-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84c45-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="84c45-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84c45-107">Definindo instância dentro da política</span><span class="sxs-lookup"><span data-stu-id="84c45-107">Setting instance within policy</span></span>


<span data-ttu-id="84c45-108">Herda [de deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="84c45-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="84c45-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="84c45-109">Properties</span></span>
|<span data-ttu-id="84c45-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84c45-110">Property</span></span>|<span data-ttu-id="84c45-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="84c45-111">Type</span></span>|<span data-ttu-id="84c45-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="84c45-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84c45-113">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="84c45-113">settingDefinitionId</span></span>|<span data-ttu-id="84c45-114">String</span><span class="sxs-lookup"><span data-stu-id="84c45-114">String</span></span>|<span data-ttu-id="84c45-115">Definição Id de definição Herdada [de deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="84c45-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="84c45-116">settingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="84c45-116">settingInstanceTemplateReference</span></span>|[<span data-ttu-id="84c45-117">deviceManagementConfigurationSettingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="84c45-117">deviceManagementConfigurationSettingInstanceTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplatereference.md)|<span data-ttu-id="84c45-118">Referência do modelo de instância de configuração Herdada [de deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="84c45-118">Setting Instance Template Reference Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="84c45-119">Relações</span><span class="sxs-lookup"><span data-stu-id="84c45-119">Relationships</span></span>
<span data-ttu-id="84c45-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="84c45-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="84c45-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="84c45-121">JSON Representation</span></span>
<span data-ttu-id="84c45-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="84c45-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingGroupCollectionInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingGroupCollectionInstance",
  "settingDefinitionId": "String",
  "settingInstanceTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
    "settingInstanceTemplateId": "String"
  }
}
```




