---
title: Tipo de recurso deviceManagementConfigurationSimpleSettingCollectionInstanceTemplate
description: Modelo de instância de conjunto de configurações simples
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4270296c68bccf831fd7dd9e0475b7e16695fc19
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664913"
---
# <a name="devicemanagementconfigurationsimplesettingcollectioninstancetemplate-resource-type"></a><span data-ttu-id="75789-103">Tipo de recurso deviceManagementConfigurationSimpleSettingCollectionInstanceTemplate</span><span class="sxs-lookup"><span data-stu-id="75789-103">deviceManagementConfigurationSimpleSettingCollectionInstanceTemplate resource type</span></span>

<span data-ttu-id="75789-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75789-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75789-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="75789-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75789-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75789-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75789-107">Modelo de instância de conjunto de configurações simples</span><span class="sxs-lookup"><span data-stu-id="75789-107">Simple Setting Collection Instance Template</span></span>


<span data-ttu-id="75789-108">Herda de [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="75789-108">Inherits from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="75789-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="75789-109">Properties</span></span>
|<span data-ttu-id="75789-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75789-110">Property</span></span>|<span data-ttu-id="75789-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="75789-111">Type</span></span>|<span data-ttu-id="75789-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="75789-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75789-113">settingInstanceTemplateId</span><span class="sxs-lookup"><span data-stu-id="75789-113">settingInstanceTemplateId</span></span>|<span data-ttu-id="75789-114">String</span><span class="sxs-lookup"><span data-stu-id="75789-114">String</span></span>|<span data-ttu-id="75789-115">Id do modelo de instância de configuração Herdada [de deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="75789-115">Setting Instance Template Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="75789-116">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="75789-116">settingDefinitionId</span></span>|<span data-ttu-id="75789-117">String</span><span class="sxs-lookup"><span data-stu-id="75789-117">String</span></span>|<span data-ttu-id="75789-118">Definição Id De definição Herdada [de deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="75789-118">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="75789-119">isRequired</span><span class="sxs-lookup"><span data-stu-id="75789-119">isRequired</span></span>|<span data-ttu-id="75789-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="75789-120">Boolean</span></span>|<span data-ttu-id="75789-121">Indica se uma política deve especificar essa configuração.</span><span class="sxs-lookup"><span data-stu-id="75789-121">Indicates if a policy must specify this setting.</span></span> <span data-ttu-id="75789-122">Herdado [de deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="75789-122">Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="75789-123">simpleSettingCollectionValueTemplate</span><span class="sxs-lookup"><span data-stu-id="75789-123">simpleSettingCollectionValueTemplate</span></span>|<span data-ttu-id="75789-124">[Coleção deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="75789-124">[deviceManagementConfigurationSimpleSettingValueTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md) collection</span></span>|<span data-ttu-id="75789-125">Modelo de valor de conjunto de configurações simples</span><span class="sxs-lookup"><span data-stu-id="75789-125">Simple Setting Collection Value Template</span></span>|
|<span data-ttu-id="75789-126">allowUnmanagedValues</span><span class="sxs-lookup"><span data-stu-id="75789-126">allowUnmanagedValues</span></span>|<span data-ttu-id="75789-127">Booleano</span><span class="sxs-lookup"><span data-stu-id="75789-127">Boolean</span></span>|<span data-ttu-id="75789-128">A política vinculada pode anexar valores que não estão presentes no modelo.</span><span class="sxs-lookup"><span data-stu-id="75789-128">Linked policy may append values which are not present in the template.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75789-129">Relações</span><span class="sxs-lookup"><span data-stu-id="75789-129">Relationships</span></span>
<span data-ttu-id="75789-130">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="75789-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="75789-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75789-131">JSON Representation</span></span>
<span data-ttu-id="75789-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="75789-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingCollectionInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true,
  "simpleSettingCollectionValueTemplate": [
    {
      "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueTemplate",
      "settingValueTemplateId": "String",
      "defaultValue": {
        "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValueConstantDefaultTemplate",
        "constantValue": "String"
      }
    }
  ],
  "allowUnmanagedValues": true
}
```




