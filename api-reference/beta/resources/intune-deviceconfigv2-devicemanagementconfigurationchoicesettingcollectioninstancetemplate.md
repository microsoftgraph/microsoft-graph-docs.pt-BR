---
title: Tipo de recurso deviceManagementConfigurationChoiceSettingCollectionInstanceTemplate
description: Modelo de instância da coleção De configuração de opção
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9f8741ab5b771325935512a179d837864a2a5b3b
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666251"
---
# <a name="devicemanagementconfigurationchoicesettingcollectioninstancetemplate-resource-type"></a><span data-ttu-id="c3472-103">Tipo de recurso deviceManagementConfigurationChoiceSettingCollectionInstanceTemplate</span><span class="sxs-lookup"><span data-stu-id="c3472-103">deviceManagementConfigurationChoiceSettingCollectionInstanceTemplate resource type</span></span>

<span data-ttu-id="c3472-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3472-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3472-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c3472-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3472-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c3472-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3472-107">Modelo de instância da coleção De configuração de opção</span><span class="sxs-lookup"><span data-stu-id="c3472-107">Choice Setting Collection Instance Template</span></span>


<span data-ttu-id="c3472-108">Herda de [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="c3472-108">Inherits from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c3472-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c3472-109">Properties</span></span>
|<span data-ttu-id="c3472-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3472-110">Property</span></span>|<span data-ttu-id="c3472-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3472-111">Type</span></span>|<span data-ttu-id="c3472-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3472-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3472-113">settingInstanceTemplateId</span><span class="sxs-lookup"><span data-stu-id="c3472-113">settingInstanceTemplateId</span></span>|<span data-ttu-id="c3472-114">String</span><span class="sxs-lookup"><span data-stu-id="c3472-114">String</span></span>|<span data-ttu-id="c3472-115">Id do modelo de instância de configuração Herdada [de deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="c3472-115">Setting Instance Template Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="c3472-116">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="c3472-116">settingDefinitionId</span></span>|<span data-ttu-id="c3472-117">String</span><span class="sxs-lookup"><span data-stu-id="c3472-117">String</span></span>|<span data-ttu-id="c3472-118">Definição Id De definição Herdada [de deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="c3472-118">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="c3472-119">isRequired</span><span class="sxs-lookup"><span data-stu-id="c3472-119">isRequired</span></span>|<span data-ttu-id="c3472-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="c3472-120">Boolean</span></span>|<span data-ttu-id="c3472-121">Indica se uma política deve especificar essa configuração.</span><span class="sxs-lookup"><span data-stu-id="c3472-121">Indicates if a policy must specify this setting.</span></span> <span data-ttu-id="c3472-122">Herdado [de deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="c3472-122">Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="c3472-123">choiceSettingCollectionValueTemplate</span><span class="sxs-lookup"><span data-stu-id="c3472-123">choiceSettingCollectionValueTemplate</span></span>|<span data-ttu-id="c3472-124">[Coleção deviceManagementConfigurationChoiceSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="c3472-124">[deviceManagementConfigurationChoiceSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluetemplate.md) collection</span></span>|<span data-ttu-id="c3472-125">Modelo de valor da coleção De configuração de opção</span><span class="sxs-lookup"><span data-stu-id="c3472-125">Choice Setting Collection Value Template</span></span>|
|<span data-ttu-id="c3472-126">allowUnmanagedValues</span><span class="sxs-lookup"><span data-stu-id="c3472-126">allowUnmanagedValues</span></span>|<span data-ttu-id="c3472-127">Booleano</span><span class="sxs-lookup"><span data-stu-id="c3472-127">Boolean</span></span>|<span data-ttu-id="c3472-128">A política vinculada pode anexar valores que não estão presentes no modelo.</span><span class="sxs-lookup"><span data-stu-id="c3472-128">Linked policy may append values which are not present in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3472-129">Relações</span><span class="sxs-lookup"><span data-stu-id="c3472-129">Relationships</span></span>
<span data-ttu-id="c3472-130">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c3472-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3472-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c3472-131">JSON Representation</span></span>
<span data-ttu-id="c3472-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c3472-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingCollectionInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingCollectionInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true,
  "choiceSettingCollectionValueTemplate": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueTemplate",
      "defaultValue": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate",
        "settingDefinitionOptionId": "String",
        "children": [
          {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
            "settingInstanceTemplateId": "String",
            "settingDefinitionId": "String",
            "isRequired": true,
            "simpleSettingValueTemplate": {
              "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
              "settingValueTemplateId": "String",
              "defaultValue": {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
                "constantValue": "String"
              }
            }
          }
        ]
      },
      "recommendedValueDefinition": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate",
        "allowedOptions": [
          {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate",
            "itemId": "String",
            "children": [
              {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
                "settingInstanceTemplateId": "String",
                "settingDefinitionId": "String",
                "isRequired": true,
                "simpleSettingValueTemplate": {
                  "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
                  "settingValueTemplateId": "String",
                  "defaultValue": {
                    "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
                    "constantValue": "String"
                  }
                }
              }
            ]
          }
        ]
      },
      "requiredValueDefinition": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate",
        "allowedOptions": [
          {
            "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate",
            "itemId": "String",
            "children": [
              {
                "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
                "settingInstanceTemplateId": "String",
                "settingDefinitionId": "String",
                "isRequired": true,
                "simpleSettingValueTemplate": {
                  "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
                  "settingValueTemplateId": "String",
                  "defaultValue": {
                    "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
                    "constantValue": "String"
                  }
                }
              }
            ]
          }
        ]
      },
      "settingValueTemplateId": "String"
    }
  ],
  "allowUnmanagedValues": true
}
```




