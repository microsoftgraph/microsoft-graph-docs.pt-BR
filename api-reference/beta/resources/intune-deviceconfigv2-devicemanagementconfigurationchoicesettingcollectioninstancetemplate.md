---
title: Tipo de recurso deviceManagementConfigurationChoiceSettingCollectionInstanceTemplate
description: Modelo de instância da coleção De configuração de opção
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 321cc8085dec3414daa1803d1c30d09dc72c79db
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868362"
---
# <a name="devicemanagementconfigurationchoicesettingcollectioninstancetemplate-resource-type"></a><span data-ttu-id="d79da-103">Tipo de recurso deviceManagementConfigurationChoiceSettingCollectionInstanceTemplate</span><span class="sxs-lookup"><span data-stu-id="d79da-103">deviceManagementConfigurationChoiceSettingCollectionInstanceTemplate resource type</span></span>

<span data-ttu-id="d79da-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d79da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d79da-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d79da-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d79da-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d79da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d79da-107">Modelo de instância da coleção De configuração de opção</span><span class="sxs-lookup"><span data-stu-id="d79da-107">Choice Setting Collection Instance Template</span></span>


<span data-ttu-id="d79da-108">Herda de [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="d79da-108">Inherits from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d79da-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d79da-109">Properties</span></span>
|<span data-ttu-id="d79da-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d79da-110">Property</span></span>|<span data-ttu-id="d79da-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d79da-111">Type</span></span>|<span data-ttu-id="d79da-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d79da-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d79da-113">settingInstanceTemplateId</span><span class="sxs-lookup"><span data-stu-id="d79da-113">settingInstanceTemplateId</span></span>|<span data-ttu-id="d79da-114">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d79da-114">String</span></span>|<span data-ttu-id="d79da-115">Id do modelo de instância de configuração Herdada [de deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="d79da-115">Setting Instance Template Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="d79da-116">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="d79da-116">settingDefinitionId</span></span>|<span data-ttu-id="d79da-117">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="d79da-117">String</span></span>|<span data-ttu-id="d79da-118">Definição Id De definição Herdada [de deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="d79da-118">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="d79da-119">isRequired</span><span class="sxs-lookup"><span data-stu-id="d79da-119">isRequired</span></span>|<span data-ttu-id="d79da-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="d79da-120">Boolean</span></span>|<span data-ttu-id="d79da-121">Indica se uma política deve especificar essa configuração.</span><span class="sxs-lookup"><span data-stu-id="d79da-121">Indicates if a policy must specify this setting.</span></span> <span data-ttu-id="d79da-122">Herdado [de deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="d79da-122">Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="d79da-123">choiceSettingCollectionValueTemplate</span><span class="sxs-lookup"><span data-stu-id="d79da-123">choiceSettingCollectionValueTemplate</span></span>|<span data-ttu-id="d79da-124">[Coleção deviceManagementConfigurationChoiceSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="d79da-124">[deviceManagementConfigurationChoiceSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluetemplate.md) collection</span></span>|<span data-ttu-id="d79da-125">Modelo de valor da coleção De configuração de opção</span><span class="sxs-lookup"><span data-stu-id="d79da-125">Choice Setting Collection Value Template</span></span>|
|<span data-ttu-id="d79da-126">allowUnmanagedValues</span><span class="sxs-lookup"><span data-stu-id="d79da-126">allowUnmanagedValues</span></span>|<span data-ttu-id="d79da-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="d79da-127">Boolean</span></span>|<span data-ttu-id="d79da-128">A política vinculada pode anexar valores que não estão presentes no modelo.</span><span class="sxs-lookup"><span data-stu-id="d79da-128">Linked policy may append values which are not present in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d79da-129">Relações</span><span class="sxs-lookup"><span data-stu-id="d79da-129">Relationships</span></span>
<span data-ttu-id="d79da-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d79da-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d79da-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d79da-131">JSON Representation</span></span>
<span data-ttu-id="d79da-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d79da-132">Here is a JSON representation of the resource.</span></span>
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
              "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValueTemplate",
              "settingValueTemplateId": "String"
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
                  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValueTemplate",
                  "settingValueTemplateId": "String"
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
                  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValueTemplate",
                  "settingValueTemplateId": "String"
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




