---
title: Tipo de recurso deviceManagementConfigurationSimpleSettingCollectionInstance
description: Instância de conjunto de configurações simples
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30dcfb5d02aebb1e7bf346c6dd1f4b37e1103b49
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664920"
---
# <a name="devicemanagementconfigurationsimplesettingcollectioninstance-resource-type"></a><span data-ttu-id="dd5bf-103">Tipo de recurso deviceManagementConfigurationSimpleSettingCollectionInstance</span><span class="sxs-lookup"><span data-stu-id="dd5bf-103">deviceManagementConfigurationSimpleSettingCollectionInstance resource type</span></span>

<span data-ttu-id="dd5bf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd5bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd5bf-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dd5bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd5bf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dd5bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd5bf-107">Instância de conjunto de configurações simples</span><span class="sxs-lookup"><span data-stu-id="dd5bf-107">Simple setting collection instance</span></span>


<span data-ttu-id="dd5bf-108">Herda [de deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="dd5bf-108">Inherits from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dd5bf-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dd5bf-109">Properties</span></span>
|<span data-ttu-id="dd5bf-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd5bf-110">Property</span></span>|<span data-ttu-id="dd5bf-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd5bf-111">Type</span></span>|<span data-ttu-id="dd5bf-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd5bf-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd5bf-113">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="dd5bf-113">settingDefinitionId</span></span>|<span data-ttu-id="dd5bf-114">String</span><span class="sxs-lookup"><span data-stu-id="dd5bf-114">String</span></span>|<span data-ttu-id="dd5bf-115">Definição Id de definição Herdada [de deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="dd5bf-115">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="dd5bf-116">settingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="dd5bf-116">settingInstanceTemplateReference</span></span>|[<span data-ttu-id="dd5bf-117">deviceManagementConfigurationSettingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="dd5bf-117">deviceManagementConfigurationSettingInstanceTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplatereference.md)|<span data-ttu-id="dd5bf-118">Referência do modelo de instância de configuração Herdada [de deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="dd5bf-118">Setting Instance Template Reference Inherited from [deviceManagementConfigurationSettingInstance](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstance.md)</span></span>|
|<span data-ttu-id="dd5bf-119">simpleSettingCollectionValue</span><span class="sxs-lookup"><span data-stu-id="dd5bf-119">simpleSettingCollectionValue</span></span>|<span data-ttu-id="dd5bf-120">[Coleção deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="dd5bf-120">[deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md) collection</span></span>|<span data-ttu-id="dd5bf-121">Valor de instância de conjunto de configurações simples</span><span class="sxs-lookup"><span data-stu-id="dd5bf-121">Simple setting collection instance value</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd5bf-122">Relações</span><span class="sxs-lookup"><span data-stu-id="dd5bf-122">Relationships</span></span>
<span data-ttu-id="dd5bf-123">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="dd5bf-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd5bf-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dd5bf-124">JSON Representation</span></span>
<span data-ttu-id="dd5bf-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dd5bf-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionInstance",
  "settingDefinitionId": "String",
  "settingInstanceTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
    "settingInstanceTemplateId": "String"
  },
  "simpleSettingCollectionValue": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValue",
      "settingValueTemplateReference": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
        "settingValueTemplateId": "String",
        "useTemplateDefault": true
      },
      "value": "String"
    }
  ]
}
```




