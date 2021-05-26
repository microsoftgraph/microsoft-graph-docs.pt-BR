---
title: Tipo de recurso deviceManagementConfigurationOptionDefinitionTemplate
description: Modelo de definição de opção
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b95ea51cab8bc3f56d7b5679743a4019e54eba54
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666510"
---
# <a name="devicemanagementconfigurationoptiondefinitiontemplate-resource-type"></a><span data-ttu-id="8726d-103">Tipo de recurso deviceManagementConfigurationOptionDefinitionTemplate</span><span class="sxs-lookup"><span data-stu-id="8726d-103">deviceManagementConfigurationOptionDefinitionTemplate resource type</span></span>

<span data-ttu-id="8726d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8726d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8726d-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8726d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8726d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8726d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8726d-107">Modelo de definição de opção</span><span class="sxs-lookup"><span data-stu-id="8726d-107">Option Definition Template</span></span>

## <a name="properties"></a><span data-ttu-id="8726d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8726d-108">Properties</span></span>
|<span data-ttu-id="8726d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8726d-109">Property</span></span>|<span data-ttu-id="8726d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8726d-110">Type</span></span>|<span data-ttu-id="8726d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8726d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8726d-112">itemId</span><span class="sxs-lookup"><span data-stu-id="8726d-112">itemId</span></span>|<span data-ttu-id="8726d-113">String</span><span class="sxs-lookup"><span data-stu-id="8726d-113">String</span></span>|<span data-ttu-id="8726d-114">ItemId de opção</span><span class="sxs-lookup"><span data-stu-id="8726d-114">Option ItemId</span></span>|
|<span data-ttu-id="8726d-115">children</span><span class="sxs-lookup"><span data-stu-id="8726d-115">children</span></span>|<span data-ttu-id="8726d-116">[Coleção deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md)</span><span class="sxs-lookup"><span data-stu-id="8726d-116">[deviceManagementConfigurationSettingInstanceTemplate](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplate.md) collection</span></span>|<span data-ttu-id="8726d-117">Opção Filhos</span><span class="sxs-lookup"><span data-stu-id="8726d-117">Option Children</span></span>|

## <a name="relationships"></a><span data-ttu-id="8726d-118">Relações</span><span class="sxs-lookup"><span data-stu-id="8726d-118">Relationships</span></span>
<span data-ttu-id="8726d-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="8726d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8726d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8726d-120">JSON Representation</span></span>
<span data-ttu-id="8726d-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8726d-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationOptionDefinitionTemplate",
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
```




