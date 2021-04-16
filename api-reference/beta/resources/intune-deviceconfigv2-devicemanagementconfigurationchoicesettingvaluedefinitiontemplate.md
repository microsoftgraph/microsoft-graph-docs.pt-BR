---
title: Tipo de recurso deviceManagementConfigurationChoiceSettingValueDefinitionTemplate
description: Modelo de definição de valor de configuração de opção
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7b4caada35c50a0d3e804a66f1556f13fbc88bfa
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868310"
---
# <a name="devicemanagementconfigurationchoicesettingvaluedefinitiontemplate-resource-type"></a><span data-ttu-id="d61d5-103">Tipo de recurso deviceManagementConfigurationChoiceSettingValueDefinitionTemplate</span><span class="sxs-lookup"><span data-stu-id="d61d5-103">deviceManagementConfigurationChoiceSettingValueDefinitionTemplate resource type</span></span>

<span data-ttu-id="d61d5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d61d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d61d5-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d61d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d61d5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d61d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d61d5-107">Modelo de definição de valor de configuração de opção</span><span class="sxs-lookup"><span data-stu-id="d61d5-107">Choice Setting Value Definition Template</span></span>

## <a name="properties"></a><span data-ttu-id="d61d5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d61d5-108">Properties</span></span>
|<span data-ttu-id="d61d5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d61d5-109">Property</span></span>|<span data-ttu-id="d61d5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d61d5-110">Type</span></span>|<span data-ttu-id="d61d5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d61d5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d61d5-112">allowedOptions</span><span class="sxs-lookup"><span data-stu-id="d61d5-112">allowedOptions</span></span>|<span data-ttu-id="d61d5-113">[Coleção deviceManagementConfigurationOptionDefinitionTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinitiontemplate.md)</span><span class="sxs-lookup"><span data-stu-id="d61d5-113">[deviceManagementConfigurationOptionDefinitionTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationoptiondefinitiontemplate.md) collection</span></span>|<span data-ttu-id="d61d5-114">Opções permitidas de configuração de opção</span><span class="sxs-lookup"><span data-stu-id="d61d5-114">Choice Setting Allowed Options</span></span>|

## <a name="relationships"></a><span data-ttu-id="d61d5-115">Relações</span><span class="sxs-lookup"><span data-stu-id="d61d5-115">Relationships</span></span>
<span data-ttu-id="d61d5-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d61d5-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d61d5-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d61d5-117">JSON Representation</span></span>
<span data-ttu-id="d61d5-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d61d5-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingValueDefinitionTemplate",
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
}
```




