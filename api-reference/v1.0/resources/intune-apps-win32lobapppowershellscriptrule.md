---
title: tipo de recurso win32LobAppPowerShellScriptRule
description: Um tipo complexo para armazenar os dados da regra de script do PowerShell para um aplicativo LOB Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 25ca86e44b6244e592214459c4ebcfbd0f228231
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020218"
---
# <a name="win32lobapppowershellscriptrule-resource-type"></a><span data-ttu-id="0cb08-103">tipo de recurso win32LobAppPowerShellScriptRule</span><span class="sxs-lookup"><span data-stu-id="0cb08-103">win32LobAppPowerShellScriptRule resource type</span></span>

<span data-ttu-id="0cb08-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cb08-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0cb08-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0cb08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cb08-106">Um tipo complexo para armazenar os dados da regra de script do PowerShell para um aplicativo LOB Win32.</span><span class="sxs-lookup"><span data-stu-id="0cb08-106">A complex type to store the PowerShell script rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="0cb08-107">Herda de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="0cb08-107">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0cb08-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0cb08-108">Properties</span></span>
|<span data-ttu-id="0cb08-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0cb08-109">Property</span></span>|<span data-ttu-id="0cb08-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0cb08-110">Type</span></span>|<span data-ttu-id="0cb08-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cb08-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cb08-112">ruleType</span><span class="sxs-lookup"><span data-stu-id="0cb08-112">ruleType</span></span>|[<span data-ttu-id="0cb08-113">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="0cb08-113">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="0cb08-114">O tipo de regra que indica o objetivo da regra.</span><span class="sxs-lookup"><span data-stu-id="0cb08-114">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="0cb08-115">Herdado de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="0cb08-115">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="0cb08-116">Os valores possíveis são: `detection` e `requirement`.</span><span class="sxs-lookup"><span data-stu-id="0cb08-116">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="0cb08-117">displayName</span><span class="sxs-lookup"><span data-stu-id="0cb08-117">displayName</span></span>|<span data-ttu-id="0cb08-118">String</span><span class="sxs-lookup"><span data-stu-id="0cb08-118">String</span></span>|<span data-ttu-id="0cb08-119">O nome de exibição da regra.</span><span class="sxs-lookup"><span data-stu-id="0cb08-119">The display name for the rule.</span></span> <span data-ttu-id="0cb08-120">Não especifique esse valor se a regra for usada para detecção.</span><span class="sxs-lookup"><span data-stu-id="0cb08-120">Do not specify this value if the rule is used for detection.</span></span>|
|<span data-ttu-id="0cb08-121">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="0cb08-121">enforceSignatureCheck</span></span>|<span data-ttu-id="0cb08-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cb08-122">Boolean</span></span>|<span data-ttu-id="0cb08-123">Um valor que indica se uma verificação de assinatura é imposta.</span><span class="sxs-lookup"><span data-stu-id="0cb08-123">A value indicating whether a signature check is enforced.</span></span>|
|<span data-ttu-id="0cb08-124">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="0cb08-124">runAs32Bit</span></span>|<span data-ttu-id="0cb08-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cb08-125">Boolean</span></span>|<span data-ttu-id="0cb08-126">Um valor que indica se o script deve ser executado como 32 bits.</span><span class="sxs-lookup"><span data-stu-id="0cb08-126">A value indicating whether the script should run as 32-bit.</span></span>|
|<span data-ttu-id="0cb08-127">scriptContent</span><span class="sxs-lookup"><span data-stu-id="0cb08-127">scriptContent</span></span>|<span data-ttu-id="0cb08-128">String</span><span class="sxs-lookup"><span data-stu-id="0cb08-128">String</span></span>|<span data-ttu-id="0cb08-129">O conteúdo de script codificado em base64.</span><span class="sxs-lookup"><span data-stu-id="0cb08-129">The base64-encoded script content.</span></span>|
|<span data-ttu-id="0cb08-130">OperationType</span><span class="sxs-lookup"><span data-stu-id="0cb08-130">operationType</span></span>|[<span data-ttu-id="0cb08-131">win32LobAppPowerShellScriptRuleOperationType</span><span class="sxs-lookup"><span data-stu-id="0cb08-131">win32LobAppPowerShellScriptRuleOperationType</span></span>](../resources/intune-apps-win32lobapppowershellscriptruleoperationtype.md)|<span data-ttu-id="0cb08-132">O tipo de operação de comparação de saída de script.</span><span class="sxs-lookup"><span data-stu-id="0cb08-132">The script output comparison operation type.</span></span> <span data-ttu-id="0cb08-133">Use não configurado (o valor padrão) se a regra for usada para detecção.</span><span class="sxs-lookup"><span data-stu-id="0cb08-133">Use NotConfigured (the default value) if the rule is used for detection.</span></span> <span data-ttu-id="0cb08-134">Os valores possíveis são: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span><span class="sxs-lookup"><span data-stu-id="0cb08-134">Possible values are: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span></span>|
|<span data-ttu-id="0cb08-135">operator</span><span class="sxs-lookup"><span data-stu-id="0cb08-135">operator</span></span>|[<span data-ttu-id="0cb08-136">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="0cb08-136">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="0cb08-137">O operador de saída de script.</span><span class="sxs-lookup"><span data-stu-id="0cb08-137">The script output operator.</span></span> <span data-ttu-id="0cb08-138">Use não configurado (o valor padrão) se a regra for usada para detecção.</span><span class="sxs-lookup"><span data-stu-id="0cb08-138">Use NotConfigured (the default value) if the rule is used for detection.</span></span> <span data-ttu-id="0cb08-139">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="0cb08-139">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="0cb08-140">ComparisonValue</span><span class="sxs-lookup"><span data-stu-id="0cb08-140">comparisonValue</span></span>|<span data-ttu-id="0cb08-141">String</span><span class="sxs-lookup"><span data-stu-id="0cb08-141">String</span></span>|<span data-ttu-id="0cb08-142">O valor de comparação de saída do script.</span><span class="sxs-lookup"><span data-stu-id="0cb08-142">The script output comparison value.</span></span> <span data-ttu-id="0cb08-143">Não especifique um valor se a regra for usada para detecção.</span><span class="sxs-lookup"><span data-stu-id="0cb08-143">Do not specify a value if the rule is used for detection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0cb08-144">Relações</span><span class="sxs-lookup"><span data-stu-id="0cb08-144">Relationships</span></span>
<span data-ttu-id="0cb08-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0cb08-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0cb08-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0cb08-146">JSON Representation</span></span>
<span data-ttu-id="0cb08-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0cb08-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptRule",
  "ruleType": "String",
  "displayName": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "scriptContent": "String",
  "operationType": "String",
  "operator": "String",
  "comparisonValue": "String"
}
```





