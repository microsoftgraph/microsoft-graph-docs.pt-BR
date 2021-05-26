---
title: Tipo de recurso deviceManagementConfigurationSimpleSettingInstance
description: Instância de configuração simples
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6c815ec0b90211ede9429abe707856af27ed79b5
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666720"
---
# <a name="devicemanagementconfigurationsimplesettinginstance-resource-type"></a><span data-ttu-id="0dbe3-103">Tipo de recurso deviceManagementConfigurationSimpleSettingInstance</span><span class="sxs-lookup"><span data-stu-id="0dbe3-103">deviceManagementConfigurationSimpleSettingInstance resource type</span></span>

<span data-ttu-id="0dbe3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0dbe3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0dbe3-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0dbe3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0dbe3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0dbe3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0dbe3-107">Instância de configuração simples</span><span class="sxs-lookup"><span data-stu-id="0dbe3-107">Simple setting instance</span></span>


<span data-ttu-id="0dbe3-108">Herda [de deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="0dbe3-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0dbe3-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0dbe3-109">Properties</span></span>
|<span data-ttu-id="0dbe3-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0dbe3-110">Property</span></span>|<span data-ttu-id="0dbe3-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="0dbe3-111">Type</span></span>|<span data-ttu-id="0dbe3-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="0dbe3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0dbe3-113">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="0dbe3-113">settingDefinitionId</span></span>|<span data-ttu-id="0dbe3-114">String</span><span class="sxs-lookup"><span data-stu-id="0dbe3-114">String</span></span>|<span data-ttu-id="0dbe3-115">Definição Id de definição Herdada [de deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="0dbe3-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="0dbe3-116">settingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="0dbe3-116">settingInstanceTemplateReference</span></span>|[<span data-ttu-id="0dbe3-117">deviceManagementConfigurationSettingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="0dbe3-117">deviceManagementConfigurationSettingInstanceTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplatereference.md)|<span data-ttu-id="0dbe3-118">Referência do modelo de instância de configuração Herdada [de deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="0dbe3-118">Setting Instance Template Reference Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="0dbe3-119">simpleSettingValue</span><span class="sxs-lookup"><span data-stu-id="0dbe3-119">simpleSettingValue</span></span>|[<span data-ttu-id="0dbe3-120">deviceManagementConfigurationSimpleSettingValue</span><span class="sxs-lookup"><span data-stu-id="0dbe3-120">deviceManagementConfigurationSimpleSettingValue</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)|<span data-ttu-id="0dbe3-121">Valor de instância de configuração simples</span><span class="sxs-lookup"><span data-stu-id="0dbe3-121">Simple setting instance value</span></span>|

## <a name="relationships"></a><span data-ttu-id="0dbe3-122">Relações</span><span class="sxs-lookup"><span data-stu-id="0dbe3-122">Relationships</span></span>
<span data-ttu-id="0dbe3-123">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="0dbe3-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0dbe3-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0dbe3-124">JSON Representation</span></span>
<span data-ttu-id="0dbe3-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0dbe3-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingInstance",
  "settingDefinitionId": "String",
  "settingInstanceTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
    "settingInstanceTemplateId": "String"
  },
  "simpleSettingValue": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValue",
    "settingValueTemplateReference": {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
      "settingValueTemplateId": "String",
      "useTemplateDefault": true
    },
    "value": "String"
  }
}
```




