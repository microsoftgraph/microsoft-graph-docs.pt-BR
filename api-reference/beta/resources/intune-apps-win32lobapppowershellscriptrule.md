---
title: tipo de recurso win32LobAppPowerShellScriptRule
description: Um tipo complexo para armazenar os dados da regra de script do PowerShell para um aplicativo LOB Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9f5d0ef733939afe0e18bbfe09db009c7631fa5f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49284579"
---
# <a name="win32lobapppowershellscriptrule-resource-type"></a><span data-ttu-id="ded40-103">tipo de recurso win32LobAppPowerShellScriptRule</span><span class="sxs-lookup"><span data-stu-id="ded40-103">win32LobAppPowerShellScriptRule resource type</span></span>

<span data-ttu-id="ded40-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ded40-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ded40-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ded40-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ded40-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ded40-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ded40-107">Um tipo complexo para armazenar os dados da regra de script do PowerShell para um aplicativo LOB Win32.</span><span class="sxs-lookup"><span data-stu-id="ded40-107">A complex type to store the PowerShell script rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="ded40-108">Herda de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="ded40-108">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ded40-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ded40-109">Properties</span></span>
|<span data-ttu-id="ded40-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ded40-110">Property</span></span>|<span data-ttu-id="ded40-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ded40-111">Type</span></span>|<span data-ttu-id="ded40-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ded40-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ded40-113">ruleType</span><span class="sxs-lookup"><span data-stu-id="ded40-113">ruleType</span></span>|[<span data-ttu-id="ded40-114">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="ded40-114">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="ded40-115">O tipo de regra que indica o objetivo da regra.</span><span class="sxs-lookup"><span data-stu-id="ded40-115">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="ded40-116">Herdado de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="ded40-116">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="ded40-117">Os valores possíveis são: `detection` e `requirement`.</span><span class="sxs-lookup"><span data-stu-id="ded40-117">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="ded40-118">displayName</span><span class="sxs-lookup"><span data-stu-id="ded40-118">displayName</span></span>|<span data-ttu-id="ded40-119">String</span><span class="sxs-lookup"><span data-stu-id="ded40-119">String</span></span>|<span data-ttu-id="ded40-120">O nome de exibição da regra.</span><span class="sxs-lookup"><span data-stu-id="ded40-120">The display name for the rule.</span></span> <span data-ttu-id="ded40-121">Não especifique esse valor se a regra for usada para detecção.</span><span class="sxs-lookup"><span data-stu-id="ded40-121">Do not specify this value if the rule is used for detection.</span></span>|
|<span data-ttu-id="ded40-122">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="ded40-122">enforceSignatureCheck</span></span>|<span data-ttu-id="ded40-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="ded40-123">Boolean</span></span>|<span data-ttu-id="ded40-124">Um valor que indica se uma verificação de assinatura é imposta.</span><span class="sxs-lookup"><span data-stu-id="ded40-124">A value indicating whether a signature check is enforced.</span></span>|
|<span data-ttu-id="ded40-125">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="ded40-125">runAs32Bit</span></span>|<span data-ttu-id="ded40-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="ded40-126">Boolean</span></span>|<span data-ttu-id="ded40-127">Um valor que indica se o script deve ser executado como 32 bits.</span><span class="sxs-lookup"><span data-stu-id="ded40-127">A value indicating whether the script should run as 32-bit.</span></span>|
|<span data-ttu-id="ded40-128">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="ded40-128">runAsAccount</span></span>|[<span data-ttu-id="ded40-129">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="ded40-129">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="ded40-130">O contexto de execução do script.</span><span class="sxs-lookup"><span data-stu-id="ded40-130">The execution context of the script.</span></span> <span data-ttu-id="ded40-131">Não especifique esse valor se a regra for usada para detecção.</span><span class="sxs-lookup"><span data-stu-id="ded40-131">Do not specify this value if the rule is used for detection.</span></span> <span data-ttu-id="ded40-132">As regras de detecção de script serão executadas no mesmo contexto do contexto de instalação de aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="ded40-132">Script detection rules will run in the same context as the associated app install context.</span></span> <span data-ttu-id="ded40-133">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="ded40-133">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="ded40-134">scriptContent</span><span class="sxs-lookup"><span data-stu-id="ded40-134">scriptContent</span></span>|<span data-ttu-id="ded40-135">String</span><span class="sxs-lookup"><span data-stu-id="ded40-135">String</span></span>|<span data-ttu-id="ded40-136">O conteúdo de script codificado em base64.</span><span class="sxs-lookup"><span data-stu-id="ded40-136">The base64-encoded script content.</span></span>|
|<span data-ttu-id="ded40-137">OperationType</span><span class="sxs-lookup"><span data-stu-id="ded40-137">operationType</span></span>|[<span data-ttu-id="ded40-138">win32LobAppPowerShellScriptRuleOperationType</span><span class="sxs-lookup"><span data-stu-id="ded40-138">win32LobAppPowerShellScriptRuleOperationType</span></span>](../resources/intune-apps-win32lobapppowershellscriptruleoperationtype.md)|<span data-ttu-id="ded40-139">O tipo de operação de comparação de saída de script.</span><span class="sxs-lookup"><span data-stu-id="ded40-139">The script output comparison operation type.</span></span> <span data-ttu-id="ded40-140">Use não configurado (o valor padrão) se a regra for usada para detecção.</span><span class="sxs-lookup"><span data-stu-id="ded40-140">Use NotConfigured (the default value) if the rule is used for detection.</span></span> <span data-ttu-id="ded40-141">Os valores possíveis são: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span><span class="sxs-lookup"><span data-stu-id="ded40-141">Possible values are: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span></span>|
|<span data-ttu-id="ded40-142">operator</span><span class="sxs-lookup"><span data-stu-id="ded40-142">operator</span></span>|[<span data-ttu-id="ded40-143">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="ded40-143">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="ded40-144">O operador de saída de script.</span><span class="sxs-lookup"><span data-stu-id="ded40-144">The script output operator.</span></span> <span data-ttu-id="ded40-145">Use não configurado (o valor padrão) se a regra for usada para detecção.</span><span class="sxs-lookup"><span data-stu-id="ded40-145">Use NotConfigured (the default value) if the rule is used for detection.</span></span> <span data-ttu-id="ded40-146">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="ded40-146">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="ded40-147">ComparisonValue</span><span class="sxs-lookup"><span data-stu-id="ded40-147">comparisonValue</span></span>|<span data-ttu-id="ded40-148">String</span><span class="sxs-lookup"><span data-stu-id="ded40-148">String</span></span>|<span data-ttu-id="ded40-149">O valor de comparação de saída do script.</span><span class="sxs-lookup"><span data-stu-id="ded40-149">The script output comparison value.</span></span> <span data-ttu-id="ded40-150">Não especifique um valor se a regra for usada para detecção.</span><span class="sxs-lookup"><span data-stu-id="ded40-150">Do not specify a value if the rule is used for detection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ded40-151">Relações</span><span class="sxs-lookup"><span data-stu-id="ded40-151">Relationships</span></span>
<span data-ttu-id="ded40-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ded40-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ded40-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ded40-153">JSON Representation</span></span>
<span data-ttu-id="ded40-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ded40-154">Here is a JSON representation of the resource.</span></span>
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
  "runAsAccount": "String",
  "scriptContent": "String",
  "operationType": "String",
  "operator": "String",
  "comparisonValue": "String"
}
```




