---
title: tipo de recurso deviceComplianceScriptRule
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 29264e89f3c935d473161edb2c4fbad3bb88849b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260257"
---
# <a name="devicecompliancescriptrule-resource-type"></a><span data-ttu-id="0d206-103">tipo de recurso deviceComplianceScriptRule</span><span class="sxs-lookup"><span data-stu-id="0d206-103">deviceComplianceScriptRule resource type</span></span>

<span data-ttu-id="0d206-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d206-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d206-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0d206-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d206-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0d206-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d206-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0d206-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="0d206-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0d206-108">Properties</span></span>
|<span data-ttu-id="0d206-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d206-109">Property</span></span>|<span data-ttu-id="0d206-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d206-110">Type</span></span>|<span data-ttu-id="0d206-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d206-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d206-112">settingName</span><span class="sxs-lookup"><span data-stu-id="0d206-112">settingName</span></span>|<span data-ttu-id="0d206-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0d206-113">String</span></span>|<span data-ttu-id="0d206-114">Nome da configuração especificado na regra.</span><span class="sxs-lookup"><span data-stu-id="0d206-114">Setting name specified in the rule.</span></span>|
|<span data-ttu-id="0d206-115">operator</span><span class="sxs-lookup"><span data-stu-id="0d206-115">operator</span></span>|[<span data-ttu-id="0d206-116">operator</span><span class="sxs-lookup"><span data-stu-id="0d206-116">operator</span></span>](../resources/intune-deviceconfig-operator.md)|<span data-ttu-id="0d206-117">Operador especificado na regra.</span><span class="sxs-lookup"><span data-stu-id="0d206-117">Operator specified in the rule.</span></span> <span data-ttu-id="0d206-118">Os valores possíveis são:,,,,,,,,,,,,,,,,,,,,,,,, `none` `and` `or` `isEquals` `notEquals` `greaterThan` `lessThan` `between` `notBetween` `greaterEquals` `lessEquals` `dayTimeBetween` `beginsWith` `notBeginsWith` `endsWith` `notEndsWith` `contains` , `notContains` , `allOf` , `oneOf` `noneOf` `setEquals` `orderedSetEquals` `subsetOf` `excludesAll` ,,,,,.</span><span class="sxs-lookup"><span data-stu-id="0d206-118">Possible values are: `none`, `and`, `or`, `isEquals`, `notEquals`, `greaterThan`, `lessThan`, `between`, `notBetween`, `greaterEquals`, `lessEquals`, `dayTimeBetween`, `beginsWith`, `notBeginsWith`, `endsWith`, `notEndsWith`, `contains`, `notContains`, `allOf`, `oneOf`, `noneOf`, `setEquals`, `orderedSetEquals`, `subsetOf`, `excludesAll`.</span></span>|
|<span data-ttu-id="0d206-119">dataType</span><span class="sxs-lookup"><span data-stu-id="0d206-119">dataType</span></span>|[<span data-ttu-id="0d206-120">dataType</span><span class="sxs-lookup"><span data-stu-id="0d206-120">dataType</span></span>](../resources/intune-deviceconfig-datatype.md)|<span data-ttu-id="0d206-121">Tipo de dados especificado na regra.</span><span class="sxs-lookup"><span data-stu-id="0d206-121">Data type specified in the rule.</span></span> <span data-ttu-id="0d206-122">Os valores possíveis são:, `none` `boolean` , `int64` , `double` , `string` , `dateTime` , `version` , `base64` , `xml` , `booleanArray` , `int64Array` , `doubleArray` ,, `stringArray` `dateTimeArray` `versionArray` .</span><span class="sxs-lookup"><span data-stu-id="0d206-122">Possible values are: `none`, `boolean`, `int64`, `double`, `string`, `dateTime`, `version`, `base64`, `xml`, `booleanArray`, `int64Array`, `doubleArray`, `stringArray`, `dateTimeArray`, `versionArray`.</span></span>|
|<span data-ttu-id="0d206-123">normaliza</span><span class="sxs-lookup"><span data-stu-id="0d206-123">operand</span></span>|<span data-ttu-id="0d206-124">String</span><span class="sxs-lookup"><span data-stu-id="0d206-124">String</span></span>|<span data-ttu-id="0d206-125">Operando especificado na regra.</span><span class="sxs-lookup"><span data-stu-id="0d206-125">Operand specified in the rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d206-126">Relações</span><span class="sxs-lookup"><span data-stu-id="0d206-126">Relationships</span></span>
<span data-ttu-id="0d206-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0d206-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d206-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0d206-128">JSON Representation</span></span>
<span data-ttu-id="0d206-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0d206-129">Here is a JSON representation of the resource.</span></span>
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




