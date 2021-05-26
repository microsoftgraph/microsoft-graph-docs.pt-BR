---
title: Tipo de recurso deviceManagementConfigurationIntegerSettingValue
description: Valor de configuração simples
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 24717f3a3d983c25198a3f94ecb5027f49f763c3
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666524"
---
# <a name="devicemanagementconfigurationintegersettingvalue-resource-type"></a><span data-ttu-id="951a5-103">Tipo de recurso deviceManagementConfigurationIntegerSettingValue</span><span class="sxs-lookup"><span data-stu-id="951a5-103">deviceManagementConfigurationIntegerSettingValue resource type</span></span>

<span data-ttu-id="951a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="951a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="951a5-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="951a5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="951a5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="951a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="951a5-107">Valor de configuração simples</span><span class="sxs-lookup"><span data-stu-id="951a5-107">Simple setting value</span></span>


<span data-ttu-id="951a5-108">Herda de [deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="951a5-108">Inherits from [deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)</span></span>

## <a name="properties"></a><span data-ttu-id="951a5-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="951a5-109">Properties</span></span>
|<span data-ttu-id="951a5-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="951a5-110">Property</span></span>|<span data-ttu-id="951a5-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="951a5-111">Type</span></span>|<span data-ttu-id="951a5-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="951a5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="951a5-113">settingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="951a5-113">settingValueTemplateReference</span></span>|[<span data-ttu-id="951a5-114">deviceManagementConfigurationSettingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="951a5-114">deviceManagementConfigurationSettingValueTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluetemplatereference.md)|<span data-ttu-id="951a5-115">Referência de modelo de valor de configuração Herdada [de deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="951a5-115">Setting value template reference Inherited from [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span></span>|
|<span data-ttu-id="951a5-116">valor</span><span class="sxs-lookup"><span data-stu-id="951a5-116">value</span></span>|<span data-ttu-id="951a5-117">Int32</span><span class="sxs-lookup"><span data-stu-id="951a5-117">Int32</span></span>|<span data-ttu-id="951a5-118">Valor da configuração de inteiro.</span><span class="sxs-lookup"><span data-stu-id="951a5-118">Value of the integer setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="951a5-119">Relações</span><span class="sxs-lookup"><span data-stu-id="951a5-119">Relationships</span></span>
<span data-ttu-id="951a5-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="951a5-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="951a5-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="951a5-121">JSON Representation</span></span>
<span data-ttu-id="951a5-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="951a5-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationIntegerSettingValue",
  "settingValueTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
    "settingValueTemplateId": "String",
    "useTemplateDefault": true
  },
  "value": 1024
}
```




