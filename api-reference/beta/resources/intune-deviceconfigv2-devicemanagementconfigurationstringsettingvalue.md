---
title: Tipo de recurso deviceManagementConfigurationStringSettingValue
description: Valor de configuração simples
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2e2374fd660fbfdcebee46ec6053d8ddc93f2010
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666699"
---
# <a name="devicemanagementconfigurationstringsettingvalue-resource-type"></a><span data-ttu-id="84e20-103">Tipo de recurso deviceManagementConfigurationStringSettingValue</span><span class="sxs-lookup"><span data-stu-id="84e20-103">deviceManagementConfigurationStringSettingValue resource type</span></span>

<span data-ttu-id="84e20-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84e20-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84e20-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="84e20-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84e20-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="84e20-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84e20-107">Valor de configuração simples</span><span class="sxs-lookup"><span data-stu-id="84e20-107">Simple setting value</span></span>


<span data-ttu-id="84e20-108">Herda de [deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="84e20-108">Inherits from [deviceManagementConfigurationSimpleSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsimplesettingvalue.md)</span></span>

## <a name="properties"></a><span data-ttu-id="84e20-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="84e20-109">Properties</span></span>
|<span data-ttu-id="84e20-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84e20-110">Property</span></span>|<span data-ttu-id="84e20-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="84e20-111">Type</span></span>|<span data-ttu-id="84e20-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="84e20-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84e20-113">settingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="84e20-113">settingValueTemplateReference</span></span>|[<span data-ttu-id="84e20-114">deviceManagementConfigurationSettingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="84e20-114">deviceManagementConfigurationSettingValueTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvaluetemplatereference.md)|<span data-ttu-id="84e20-115">Referência de modelo de valor de configuração Herdada [de deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="84e20-115">Setting value template reference Inherited from [deviceManagementConfigurationSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettingvalue.md)</span></span>|
|<span data-ttu-id="84e20-116">value</span><span class="sxs-lookup"><span data-stu-id="84e20-116">value</span></span>|<span data-ttu-id="84e20-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84e20-117">String</span></span>|<span data-ttu-id="84e20-118">Valor da configuração da cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="84e20-118">Value of the string setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84e20-119">Relações</span><span class="sxs-lookup"><span data-stu-id="84e20-119">Relationships</span></span>
<span data-ttu-id="84e20-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="84e20-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="84e20-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="84e20-121">JSON Representation</span></span>
<span data-ttu-id="84e20-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="84e20-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationStringSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationStringSettingValue",
  "settingValueTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
    "settingValueTemplateId": "String",
    "useTemplateDefault": true
  },
  "value": "String"
}
```




