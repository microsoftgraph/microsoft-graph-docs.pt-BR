---
title: Tipo de recurso deviceManagementConfigurationSimpleSettingValue
description: Valor de configuração simples
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1f56883a53cab24f9859e968c11827a7a104a776
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666706"
---
# <a name="devicemanagementconfigurationsimplesettingvalue-resource-type"></a><span data-ttu-id="cb0bb-103">Tipo de recurso deviceManagementConfigurationSimpleSettingValue</span><span class="sxs-lookup"><span data-stu-id="cb0bb-103">deviceManagementConfigurationSimpleSettingValue resource type</span></span>

<span data-ttu-id="cb0bb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb0bb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb0bb-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cb0bb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb0bb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cb0bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb0bb-107">Valor de configuração simples</span><span class="sxs-lookup"><span data-stu-id="cb0bb-107">Simple setting value</span></span>


<span data-ttu-id="cb0bb-108">Herda de [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="cb0bb-108">Inherits from [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cb0bb-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cb0bb-109">Properties</span></span>
|<span data-ttu-id="cb0bb-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cb0bb-110">Property</span></span>|<span data-ttu-id="cb0bb-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="cb0bb-111">Type</span></span>|<span data-ttu-id="cb0bb-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb0bb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb0bb-113">settingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="cb0bb-113">settingValueTemplateReference</span></span>|[<span data-ttu-id="cb0bb-114">deviceManagementConfigurationSettingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="cb0bb-114">deviceManagementConfigurationSettingValueTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluetemplatereference.md)|<span data-ttu-id="cb0bb-115">Referência de modelo de valor de configuração Herdada [de deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="cb0bb-115">Setting value template reference Inherited from [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb0bb-116">Relações</span><span class="sxs-lookup"><span data-stu-id="cb0bb-116">Relationships</span></span>
<span data-ttu-id="cb0bb-117">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="cb0bb-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb0bb-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cb0bb-118">JSON Representation</span></span>
<span data-ttu-id="cb0bb-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cb0bb-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSimpleSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSimpleSettingValue",
  "settingValueTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
    "settingValueTemplateId": "String",
    "useTemplateDefault": true
  }
}
```




