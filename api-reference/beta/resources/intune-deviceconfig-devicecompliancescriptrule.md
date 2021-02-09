---
title: Tipo de recurso deviceComplianceScriptRule
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 169c286043e4c1ec7b9b16e45fa6fb4520781211
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154898"
---
# <a name="devicecompliancescriptrule-resource-type"></a><span data-ttu-id="e35a1-103">Tipo de recurso deviceComplianceScriptRule</span><span class="sxs-lookup"><span data-stu-id="e35a1-103">deviceComplianceScriptRule resource type</span></span>

<span data-ttu-id="e35a1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e35a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e35a1-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e35a1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e35a1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e35a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e35a1-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e35a1-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e35a1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e35a1-108">Properties</span></span>
|<span data-ttu-id="e35a1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e35a1-109">Property</span></span>|<span data-ttu-id="e35a1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e35a1-110">Type</span></span>|<span data-ttu-id="e35a1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e35a1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e35a1-112">settingName</span><span class="sxs-lookup"><span data-stu-id="e35a1-112">settingName</span></span>|<span data-ttu-id="e35a1-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e35a1-113">String</span></span>|<span data-ttu-id="e35a1-114">Nome da configuração especificado na regra.</span><span class="sxs-lookup"><span data-stu-id="e35a1-114">Setting name specified in the rule.</span></span>|
|<span data-ttu-id="e35a1-115">operator</span><span class="sxs-lookup"><span data-stu-id="e35a1-115">operator</span></span>|[<span data-ttu-id="e35a1-116">operator</span><span class="sxs-lookup"><span data-stu-id="e35a1-116">operator</span></span>](../resources/intune-deviceconfig-operator.md)|<span data-ttu-id="e35a1-117">Operador especificado na regra.</span><span class="sxs-lookup"><span data-stu-id="e35a1-117">Operator specified in the rule.</span></span> <span data-ttu-id="e35a1-118">Os valores possíveis `none` são: `and` , , , , , , , , `or` `isEquals` , , `notEquals` `greaterThan` , , `lessThan` `between` , `notBetween` `greaterEquals` `lessEquals` `dayTimeBetween` `beginsWith` `notBeginsWith` , `endsWith` `notEndsWith` `contains` `notContains` `allOf` `oneOf` `noneOf` `setEquals` `orderedSetEquals` `subsetOf` `excludesAll` .</span><span class="sxs-lookup"><span data-stu-id="e35a1-118">Possible values are: `none`, `and`, `or`, `isEquals`, `notEquals`, `greaterThan`, `lessThan`, `between`, `notBetween`, `greaterEquals`, `lessEquals`, `dayTimeBetween`, `beginsWith`, `notBeginsWith`, `endsWith`, `notEndsWith`, `contains`, `notContains`, `allOf`, `oneOf`, `noneOf`, `setEquals`, `orderedSetEquals`, `subsetOf`, `excludesAll`.</span></span>|
|<span data-ttu-id="e35a1-119">deviceComplianceScriptRulOperator</span><span class="sxs-lookup"><span data-stu-id="e35a1-119">deviceComplianceScriptRulOperator</span></span>|[<span data-ttu-id="e35a1-120">deviceComplianceScriptRulOperator</span><span class="sxs-lookup"><span data-stu-id="e35a1-120">deviceComplianceScriptRulOperator</span></span>](../resources/intune-deviceconfig-devicecompliancescriptruloperator.md)|<span data-ttu-id="e35a1-121">Operador especificado na regra.</span><span class="sxs-lookup"><span data-stu-id="e35a1-121">Operator specified in the rule.</span></span> <span data-ttu-id="e35a1-122">Os valores possíveis `none` são: `and` , , , , , , `or` , `isEquals` `notEquals` , , , `greaterThan` , , `lessThan` , `between` `notBetween` `greaterEquals` `lessEquals` `dayTimeBetween` `beginsWith` `notBeginsWith` , `endsWith` `notEndsWith` `contains` `notContains` `allOf` `oneOf` `noneOf` `setEquals` `orderedSetEquals` `subsetOf` `excludesAll` .</span><span class="sxs-lookup"><span data-stu-id="e35a1-122">Possible values are: `none`, `and`, `or`, `isEquals`, `notEquals`, `greaterThan`, `lessThan`, `between`, `notBetween`, `greaterEquals`, `lessEquals`, `dayTimeBetween`, `beginsWith`, `notBeginsWith`, `endsWith`, `notEndsWith`, `contains`, `notContains`, `allOf`, `oneOf`, `noneOf`, `setEquals`, `orderedSetEquals`, `subsetOf`, `excludesAll`.</span></span>|
|<span data-ttu-id="e35a1-123">dataType</span><span class="sxs-lookup"><span data-stu-id="e35a1-123">dataType</span></span>|[<span data-ttu-id="e35a1-124">dataType</span><span class="sxs-lookup"><span data-stu-id="e35a1-124">dataType</span></span>](../resources/intune-deviceconfig-datatype.md)|<span data-ttu-id="e35a1-125">Tipo de dados especificado na regra.</span><span class="sxs-lookup"><span data-stu-id="e35a1-125">Data type specified in the rule.</span></span> <span data-ttu-id="e35a1-126">Os valores possíveis `none` são: `boolean` , , , , , , , , `int64` , , `double` , , , `string` , `dateTime` `version` `base64` `xml` `booleanArray` `int64Array` `doubleArray` `stringArray` `dateTimeArray` `versionArray` .</span><span class="sxs-lookup"><span data-stu-id="e35a1-126">Possible values are: `none`, `boolean`, `int64`, `double`, `string`, `dateTime`, `version`, `base64`, `xml`, `booleanArray`, `int64Array`, `doubleArray`, `stringArray`, `dateTimeArray`, `versionArray`.</span></span>|
|<span data-ttu-id="e35a1-127">deviceComplianceScriptRuleDataType</span><span class="sxs-lookup"><span data-stu-id="e35a1-127">deviceComplianceScriptRuleDataType</span></span>|[<span data-ttu-id="e35a1-128">deviceComplianceScriptRuleDataType</span><span class="sxs-lookup"><span data-stu-id="e35a1-128">deviceComplianceScriptRuleDataType</span></span>](../resources/intune-deviceconfig-devicecompliancescriptruledatatype.md)|<span data-ttu-id="e35a1-129">Tipo de dados especificado na regra.</span><span class="sxs-lookup"><span data-stu-id="e35a1-129">Data type specified in the rule.</span></span> <span data-ttu-id="e35a1-130">Os valores possíveis `none` são: `boolean` , , , , , , , , `int64` , , `double` , , , `string` , `dateTime` `version` `base64` `xml` `booleanArray` `int64Array` `doubleArray` `stringArray` `dateTimeArray` `versionArray` .</span><span class="sxs-lookup"><span data-stu-id="e35a1-130">Possible values are: `none`, `boolean`, `int64`, `double`, `string`, `dateTime`, `version`, `base64`, `xml`, `booleanArray`, `int64Array`, `doubleArray`, `stringArray`, `dateTimeArray`, `versionArray`.</span></span>|
|<span data-ttu-id="e35a1-131">operand</span><span class="sxs-lookup"><span data-stu-id="e35a1-131">operand</span></span>|<span data-ttu-id="e35a1-132">String</span><span class="sxs-lookup"><span data-stu-id="e35a1-132">String</span></span>|<span data-ttu-id="e35a1-133">Opernd especificado na regra.</span><span class="sxs-lookup"><span data-stu-id="e35a1-133">Operand specified in the rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e35a1-134">Relações</span><span class="sxs-lookup"><span data-stu-id="e35a1-134">Relationships</span></span>
<span data-ttu-id="e35a1-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e35a1-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e35a1-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e35a1-136">JSON Representation</span></span>
<span data-ttu-id="e35a1-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e35a1-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceComplianceScriptRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRule",
  "settingName": "String",
  "operator": "String",
  "deviceComplianceScriptRulOperator": "String",
  "dataType": "String",
  "deviceComplianceScriptRuleDataType": "String",
  "operand": "String"
}
```




