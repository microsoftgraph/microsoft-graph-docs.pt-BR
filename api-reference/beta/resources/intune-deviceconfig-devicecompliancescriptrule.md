---
title: tipo de recurso deviceComplianceScriptRule
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c5c524202b8e15d077895c47c1c66256d58ca2c3
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44789295"
---
# <a name="devicecompliancescriptrule-resource-type"></a><span data-ttu-id="f1de2-103">tipo de recurso deviceComplianceScriptRule</span><span class="sxs-lookup"><span data-stu-id="f1de2-103">deviceComplianceScriptRule resource type</span></span>

<span data-ttu-id="f1de2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1de2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f1de2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f1de2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1de2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f1de2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1de2-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f1de2-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f1de2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f1de2-108">Properties</span></span>
|<span data-ttu-id="f1de2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1de2-109">Property</span></span>|<span data-ttu-id="f1de2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1de2-110">Type</span></span>|<span data-ttu-id="f1de2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1de2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1de2-112">settingName</span><span class="sxs-lookup"><span data-stu-id="f1de2-112">settingName</span></span>|<span data-ttu-id="f1de2-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1de2-113">String</span></span>|<span data-ttu-id="f1de2-114">Nome da configuração especificado na regra.</span><span class="sxs-lookup"><span data-stu-id="f1de2-114">Setting name specified in the rule.</span></span>|
|<span data-ttu-id="f1de2-115">operator</span><span class="sxs-lookup"><span data-stu-id="f1de2-115">operator</span></span>|[<span data-ttu-id="f1de2-116">operador</span><span class="sxs-lookup"><span data-stu-id="f1de2-116">operator</span></span>](../resources/intune-deviceconfig-operator.md)|<span data-ttu-id="f1de2-117">Operador especificado na regra.</span><span class="sxs-lookup"><span data-stu-id="f1de2-117">Operator specified in the rule.</span></span> <span data-ttu-id="f1de2-118">Os valores possíveis são:,,,,,,,,,,,,,,,,,,,,,,,, `none` `and` `or` `isEquals` `notEquals` `greaterThan` `lessThan` `between` `notBetween` `greaterEquals` `lessEquals` `dayTimeBetween` `beginsWith` `notBeginsWith` `endsWith` `notEndsWith` `contains` , `notContains` , `allOf` , `oneOf` `noneOf` `setEquals` `orderedSetEquals` `subsetOf` `excludesAll` ,,,,,.</span><span class="sxs-lookup"><span data-stu-id="f1de2-118">Possible values are: `none`, `and`, `or`, `isEquals`, `notEquals`, `greaterThan`, `lessThan`, `between`, `notBetween`, `greaterEquals`, `lessEquals`, `dayTimeBetween`, `beginsWith`, `notBeginsWith`, `endsWith`, `notEndsWith`, `contains`, `notContains`, `allOf`, `oneOf`, `noneOf`, `setEquals`, `orderedSetEquals`, `subsetOf`, `excludesAll`.</span></span>|
|<span data-ttu-id="f1de2-119">dataType</span><span class="sxs-lookup"><span data-stu-id="f1de2-119">dataType</span></span>|[<span data-ttu-id="f1de2-120">Alinha</span><span class="sxs-lookup"><span data-stu-id="f1de2-120">dataType</span></span>](../resources/intune-deviceconfig-datatype.md)|<span data-ttu-id="f1de2-121">Tipo de dados especificado na regra.</span><span class="sxs-lookup"><span data-stu-id="f1de2-121">Data type specified in the rule.</span></span> <span data-ttu-id="f1de2-122">Os valores possíveis são:, `none` `boolean` , `int64` , `double` , `string` , `dateTime` , `version` , `base64` , `xml` , `booleanArray` , `int64Array` , `doubleArray` ,, `stringArray` `dateTimeArray` `versionArray` .</span><span class="sxs-lookup"><span data-stu-id="f1de2-122">Possible values are: `none`, `boolean`, `int64`, `double`, `string`, `dateTime`, `version`, `base64`, `xml`, `booleanArray`, `int64Array`, `doubleArray`, `stringArray`, `dateTimeArray`, `versionArray`.</span></span>|
|<span data-ttu-id="f1de2-123">normaliza</span><span class="sxs-lookup"><span data-stu-id="f1de2-123">operand</span></span>|<span data-ttu-id="f1de2-124">String</span><span class="sxs-lookup"><span data-stu-id="f1de2-124">String</span></span>|<span data-ttu-id="f1de2-125">Operando especificado na regra.</span><span class="sxs-lookup"><span data-stu-id="f1de2-125">Operand specified in the rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1de2-126">Relações</span><span class="sxs-lookup"><span data-stu-id="f1de2-126">Relationships</span></span>
<span data-ttu-id="f1de2-127">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="f1de2-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1de2-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f1de2-128">JSON Representation</span></span>
<span data-ttu-id="f1de2-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f1de2-129">Here is a JSON representation of the resource.</span></span>
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
  "dataType": "String",
  "operand": "String"
}
```



