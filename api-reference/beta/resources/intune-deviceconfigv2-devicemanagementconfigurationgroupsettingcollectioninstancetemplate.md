---
title: Tipo de recurso deviceManagementConfigurationGroupSettingCollectionInstanceTemplate
description: Modelo de instância de conjunto de configurações de grupo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1a1b4b750b69521a055f5c82004db28e0bf8b52b
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868305"
---
# <a name="devicemanagementconfigurationgroupsettingcollectioninstancetemplate-resource-type"></a><span data-ttu-id="880b1-103">Tipo de recurso deviceManagementConfigurationGroupSettingCollectionInstanceTemplate</span><span class="sxs-lookup"><span data-stu-id="880b1-103">deviceManagementConfigurationGroupSettingCollectionInstanceTemplate resource type</span></span>

<span data-ttu-id="880b1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="880b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="880b1-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="880b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="880b1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="880b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="880b1-107">Modelo de instância de conjunto de configurações de grupo</span><span class="sxs-lookup"><span data-stu-id="880b1-107">Group Setting Collection Instance Template</span></span>


<span data-ttu-id="880b1-108">Herda de [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="880b1-108">Inherits from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="880b1-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="880b1-109">Properties</span></span>
|<span data-ttu-id="880b1-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="880b1-110">Property</span></span>|<span data-ttu-id="880b1-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="880b1-111">Type</span></span>|<span data-ttu-id="880b1-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="880b1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="880b1-113">settingInstanceTemplateId</span><span class="sxs-lookup"><span data-stu-id="880b1-113">settingInstanceTemplateId</span></span>|<span data-ttu-id="880b1-114">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="880b1-114">String</span></span>|<span data-ttu-id="880b1-115">Id do modelo de instância de configuração Herdada [de deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="880b1-115">Setting Instance Template Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="880b1-116">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="880b1-116">settingDefinitionId</span></span>|<span data-ttu-id="880b1-117">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="880b1-117">String</span></span>|<span data-ttu-id="880b1-118">Definição Id De definição Herdada [de deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="880b1-118">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="880b1-119">isRequired</span><span class="sxs-lookup"><span data-stu-id="880b1-119">isRequired</span></span>|<span data-ttu-id="880b1-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="880b1-120">Boolean</span></span>|<span data-ttu-id="880b1-121">Indica se uma política deve especificar essa configuração.</span><span class="sxs-lookup"><span data-stu-id="880b1-121">Indicates if a policy must specify this setting.</span></span> <span data-ttu-id="880b1-122">Herdado [de deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="880b1-122">Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="880b1-123">groupSettingCollectionValueTemplate</span><span class="sxs-lookup"><span data-stu-id="880b1-123">groupSettingCollectionValueTemplate</span></span>|<span data-ttu-id="880b1-124">[Coleção deviceManagementConfigurationGroupSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationgroupsettingvaluetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="880b1-124">[deviceManagementConfigurationGroupSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationgroupsettingvaluetemplate.md) collection</span></span>|<span data-ttu-id="880b1-125">Modelo de valor da coleção de configurações de grupo</span><span class="sxs-lookup"><span data-stu-id="880b1-125">Group Setting Collection Value Template</span></span>|
|<span data-ttu-id="880b1-126">allowUnmanagedValues</span><span class="sxs-lookup"><span data-stu-id="880b1-126">allowUnmanagedValues</span></span>|<span data-ttu-id="880b1-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="880b1-127">Boolean</span></span>|<span data-ttu-id="880b1-128">A política vinculada pode anexar valores que não estão presentes no modelo.</span><span class="sxs-lookup"><span data-stu-id="880b1-128">Linked policy may append values which are not present in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="880b1-129">Relações</span><span class="sxs-lookup"><span data-stu-id="880b1-129">Relationships</span></span>
<span data-ttu-id="880b1-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="880b1-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="880b1-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="880b1-131">JSON Representation</span></span>
<span data-ttu-id="880b1-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="880b1-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingCollectionInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationGroupSettingCollectionInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true,
  "groupSettingCollectionValueTemplate": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingValueTemplate",
      "children": [
        {
          "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
          "settingInstanceTemplateId": "String",
          "settingDefinitionId": "String",
          "isRequired": true,
          "simpleSettingValueTemplate": {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValueTemplate",
            "settingValueTemplateId": "String"
          }
        }
      ],
      "settingValueTemplateId": "String"
    }
  ],
  "allowUnmanagedValues": true
}
```




