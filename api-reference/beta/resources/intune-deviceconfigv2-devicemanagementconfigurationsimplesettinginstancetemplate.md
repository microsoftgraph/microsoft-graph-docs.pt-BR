---
title: Tipo de recurso deviceManagementConfigurationSimpleSettingInstanceTemplate
description: Modelo de instância de configuração simples
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b09e26ef14e20c1cbc95013beb09f9111ddf123e
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868294"
---
# <a name="devicemanagementconfigurationsimplesettinginstancetemplate-resource-type"></a><span data-ttu-id="87864-103">Tipo de recurso deviceManagementConfigurationSimpleSettingInstanceTemplate</span><span class="sxs-lookup"><span data-stu-id="87864-103">deviceManagementConfigurationSimpleSettingInstanceTemplate resource type</span></span>

<span data-ttu-id="87864-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87864-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87864-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="87864-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87864-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="87864-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87864-107">Modelo de instância de configuração simples</span><span class="sxs-lookup"><span data-stu-id="87864-107">Simple Setting Instance Template</span></span>


<span data-ttu-id="87864-108">Herda de [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="87864-108">Inherits from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="87864-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87864-109">Properties</span></span>
|<span data-ttu-id="87864-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87864-110">Property</span></span>|<span data-ttu-id="87864-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="87864-111">Type</span></span>|<span data-ttu-id="87864-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="87864-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87864-113">settingInstanceTemplateId</span><span class="sxs-lookup"><span data-stu-id="87864-113">settingInstanceTemplateId</span></span>|<span data-ttu-id="87864-114">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="87864-114">String</span></span>|<span data-ttu-id="87864-115">Id do modelo de instância de configuração Herdada [de deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="87864-115">Setting Instance Template Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="87864-116">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="87864-116">settingDefinitionId</span></span>|<span data-ttu-id="87864-117">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="87864-117">String</span></span>|<span data-ttu-id="87864-118">Definição Id De definição Herdada [de deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="87864-118">Setting Definition Id Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="87864-119">isRequired</span><span class="sxs-lookup"><span data-stu-id="87864-119">isRequired</span></span>|<span data-ttu-id="87864-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="87864-120">Boolean</span></span>|<span data-ttu-id="87864-121">Indica se uma política deve especificar essa configuração.</span><span class="sxs-lookup"><span data-stu-id="87864-121">Indicates if a policy must specify this setting.</span></span> <span data-ttu-id="87864-122">Herdado [de deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="87864-122">Inherited from [deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span></span>|
|<span data-ttu-id="87864-123">simpleSettingValueTemplate</span><span class="sxs-lookup"><span data-stu-id="87864-123">simpleSettingValueTemplate</span></span>|[<span data-ttu-id="87864-124">deviceManagementConfigurationSimpleSettingValueTemplate</span><span class="sxs-lookup"><span data-stu-id="87864-124">deviceManagementConfigurationSimpleSettingValueTemplate</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvaluetemplate.md)|<span data-ttu-id="87864-125">Modelo de valor de configuração simples</span><span class="sxs-lookup"><span data-stu-id="87864-125">Simple Setting Value Template</span></span>|

## <a name="relationships"></a><span data-ttu-id="87864-126">Relações</span><span class="sxs-lookup"><span data-stu-id="87864-126">Relationships</span></span>
<span data-ttu-id="87864-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="87864-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="87864-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87864-128">JSON Representation</span></span>
<span data-ttu-id="87864-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="87864-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true,
  "simpleSettingValueTemplate": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValueTemplate",
    "settingValueTemplateId": "String"
  }
}
```




