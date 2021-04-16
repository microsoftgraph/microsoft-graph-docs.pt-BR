---
title: Tipo de recurso deviceManagementConfigurationGroupSettingValueTemplate
description: Modelo de valor de configuração de grupo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 510abd102fda4721a387359afbeaa870abac6be8
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868302"
---
# <a name="devicemanagementconfigurationgroupsettingvaluetemplate-resource-type"></a><span data-ttu-id="c0c89-103">Tipo de recurso deviceManagementConfigurationGroupSettingValueTemplate</span><span class="sxs-lookup"><span data-stu-id="c0c89-103">deviceManagementConfigurationGroupSettingValueTemplate resource type</span></span>

<span data-ttu-id="c0c89-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0c89-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0c89-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c0c89-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0c89-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c0c89-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0c89-107">Modelo de valor de configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="c0c89-107">Group Setting Value Template</span></span>

## <a name="properties"></a><span data-ttu-id="c0c89-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c0c89-108">Properties</span></span>
|<span data-ttu-id="c0c89-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0c89-109">Property</span></span>|<span data-ttu-id="c0c89-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0c89-110">Type</span></span>|<span data-ttu-id="c0c89-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0c89-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0c89-112">filhos</span><span class="sxs-lookup"><span data-stu-id="c0c89-112">children</span></span>|<span data-ttu-id="c0c89-113">[Coleção deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="c0c89-113">[deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md) collection</span></span>|<span data-ttu-id="c0c89-114">Filhos do valor da configuração de grupo</span><span class="sxs-lookup"><span data-stu-id="c0c89-114">Group setting value children</span></span>|
|<span data-ttu-id="c0c89-115">settingValueTemplateId</span><span class="sxs-lookup"><span data-stu-id="c0c89-115">settingValueTemplateId</span></span>|<span data-ttu-id="c0c89-116">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="c0c89-116">String</span></span>|<span data-ttu-id="c0c89-117">Definindo a ID do Modelo de Valor</span><span class="sxs-lookup"><span data-stu-id="c0c89-117">Setting Value Template Id</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0c89-118">Relações</span><span class="sxs-lookup"><span data-stu-id="c0c89-118">Relationships</span></span>
<span data-ttu-id="c0c89-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c0c89-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0c89-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c0c89-120">JSON Representation</span></span>
<span data-ttu-id="c0c89-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c0c89-121">Here is a JSON representation of the resource.</span></span>
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
        "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValueTemplate",
        "settingValueTemplateId": "String"
      }
    }
  ],
  "settingValueTemplateId": "String"
}
```




