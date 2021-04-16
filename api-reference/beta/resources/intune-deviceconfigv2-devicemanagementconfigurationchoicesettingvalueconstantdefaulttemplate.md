---
title: Tipo de recurso deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate
description: Modelo padrão de constante de valor de configuração de opção
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8b74dbf6552fda605708dbd5f197f5ee0167d2ac
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868316"
---
# <a name="devicemanagementconfigurationchoicesettingvalueconstantdefaulttemplate-resource-type"></a><span data-ttu-id="83c71-103">Tipo de recurso deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate</span><span class="sxs-lookup"><span data-stu-id="83c71-103">deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate resource type</span></span>

<span data-ttu-id="83c71-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83c71-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83c71-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="83c71-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83c71-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="83c71-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83c71-107">Modelo padrão de constante de valor de configuração de opção</span><span class="sxs-lookup"><span data-stu-id="83c71-107">Choice Setting Value Constant Default Template</span></span>


<span data-ttu-id="83c71-108">Herda [de deviceManagementConfigurationChoiceSettingValueDefaultTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefaulttemplate.md)</span><span class="sxs-lookup"><span data-stu-id="83c71-108">Inherits from [deviceManagementConfigurationChoiceSettingValueDefaultTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationchoicesettingvaluedefaulttemplate.md)</span></span>

## <a name="properties"></a><span data-ttu-id="83c71-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="83c71-109">Properties</span></span>
|<span data-ttu-id="83c71-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="83c71-110">Property</span></span>|<span data-ttu-id="83c71-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="83c71-111">Type</span></span>|<span data-ttu-id="83c71-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="83c71-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83c71-113">settingDefinitionOptionId</span><span class="sxs-lookup"><span data-stu-id="83c71-113">settingDefinitionOptionId</span></span>|<span data-ttu-id="83c71-114">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="83c71-114">String</span></span>|<span data-ttu-id="83c71-115">Valor constante padrão</span><span class="sxs-lookup"><span data-stu-id="83c71-115">Default Constant Value</span></span>|
|<span data-ttu-id="83c71-116">children</span><span class="sxs-lookup"><span data-stu-id="83c71-116">children</span></span>|<span data-ttu-id="83c71-117">[Coleção deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="83c71-117">[deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md) collection</span></span>|<span data-ttu-id="83c71-118">Opção Filhos</span><span class="sxs-lookup"><span data-stu-id="83c71-118">Option Children</span></span>|

## <a name="relationships"></a><span data-ttu-id="83c71-119">Relações</span><span class="sxs-lookup"><span data-stu-id="83c71-119">Relationships</span></span>
<span data-ttu-id="83c71-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="83c71-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83c71-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="83c71-121">JSON Representation</span></span>
<span data-ttu-id="83c71-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="83c71-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationChoiceSettingValueConstantDefaultTemplate",
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
}
```




