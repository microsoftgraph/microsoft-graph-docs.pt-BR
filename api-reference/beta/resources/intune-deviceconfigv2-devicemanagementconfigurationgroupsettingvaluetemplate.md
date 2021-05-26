---
title: Tipo de recurso deviceManagementConfigurationGroupSettingValueTemplate
description: Modelo de valor de configuração de grupo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: aa840fe5755955d8d1649f64f4b0ea610bd53cd0
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666531"
---
# <a name="devicemanagementconfigurationgroupsettingvaluetemplate-resource-type"></a><span data-ttu-id="42462-103">Tipo de recurso deviceManagementConfigurationGroupSettingValueTemplate</span><span class="sxs-lookup"><span data-stu-id="42462-103">deviceManagementConfigurationGroupSettingValueTemplate resource type</span></span>

<span data-ttu-id="42462-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42462-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42462-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="42462-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42462-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="42462-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42462-107">Modelo de valor de configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="42462-107">Group Setting Value Template</span></span>

## <a name="properties"></a><span data-ttu-id="42462-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="42462-108">Properties</span></span>
|<span data-ttu-id="42462-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42462-109">Property</span></span>|<span data-ttu-id="42462-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="42462-110">Type</span></span>|<span data-ttu-id="42462-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="42462-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42462-112">filhos</span><span class="sxs-lookup"><span data-stu-id="42462-112">children</span></span>|<span data-ttu-id="42462-113">[Coleção deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="42462-113">[deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md) collection</span></span>|<span data-ttu-id="42462-114">Filhos do valor da configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="42462-114">Group setting value children</span></span>|
|<span data-ttu-id="42462-115">settingValueTemplateId</span><span class="sxs-lookup"><span data-stu-id="42462-115">settingValueTemplateId</span></span>|<span data-ttu-id="42462-116">String</span><span class="sxs-lookup"><span data-stu-id="42462-116">String</span></span>|<span data-ttu-id="42462-117">Definindo a ID do Modelo de Valor</span><span class="sxs-lookup"><span data-stu-id="42462-117">Setting Value Template Id</span></span>|

## <a name="relationships"></a><span data-ttu-id="42462-118">Relações</span><span class="sxs-lookup"><span data-stu-id="42462-118">Relationships</span></span>
<span data-ttu-id="42462-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="42462-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="42462-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="42462-120">JSON Representation</span></span>
<span data-ttu-id="42462-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="42462-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationGroupSettingValueTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationGroupSettingValueTemplate",
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
  ],
  "settingValueTemplateId": "String"
}
```




