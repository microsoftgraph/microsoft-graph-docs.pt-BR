---
title: tipo de recurso win32LobAppPowerShellScriptRule
description: Um tipo complexo para armazenar os dados da regra de script do PowerShell para um aplicativo LOB Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c392d43f6e9836118f1d32320c5e63498226fed9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48712061"
---
# <a name="win32lobapppowershellscriptrule-resource-type"></a><span data-ttu-id="e79c7-103">tipo de recurso win32LobAppPowerShellScriptRule</span><span class="sxs-lookup"><span data-stu-id="e79c7-103">win32LobAppPowerShellScriptRule resource type</span></span>

<span data-ttu-id="e79c7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e79c7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e79c7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e79c7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e79c7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e79c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e79c7-107">Um tipo complexo para armazenar os dados da regra de script do PowerShell para um aplicativo LOB Win32.</span><span class="sxs-lookup"><span data-stu-id="e79c7-107">A complex type to store the PowerShell script rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="e79c7-108">Herda de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="e79c7-108">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e79c7-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e79c7-109">Properties</span></span>
|<span data-ttu-id="e79c7-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e79c7-110">Property</span></span>|<span data-ttu-id="e79c7-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e79c7-111">Type</span></span>|<span data-ttu-id="e79c7-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e79c7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e79c7-113">ruleType</span><span class="sxs-lookup"><span data-stu-id="e79c7-113">ruleType</span></span>|[<span data-ttu-id="e79c7-114">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="e79c7-114">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="e79c7-115">O tipo de regra que indica o objetivo da regra.</span><span class="sxs-lookup"><span data-stu-id="e79c7-115">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="e79c7-116">Herdado de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="e79c7-116">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="e79c7-117">Os valores possíveis são: `detection` e `requirement`.</span><span class="sxs-lookup"><span data-stu-id="e79c7-117">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="e79c7-118">displayName</span><span class="sxs-lookup"><span data-stu-id="e79c7-118">displayName</span></span>|<span data-ttu-id="e79c7-119">String</span><span class="sxs-lookup"><span data-stu-id="e79c7-119">String</span></span>|<span data-ttu-id="e79c7-120">O nome de exibição da regra.</span><span class="sxs-lookup"><span data-stu-id="e79c7-120">The display name for the rule.</span></span> <span data-ttu-id="e79c7-121">Não especifique esse valor se a regra for usada para detecção.</span><span class="sxs-lookup"><span data-stu-id="e79c7-121">Do not specify this value if the rule is used for detection.</span></span>|
|<span data-ttu-id="e79c7-122">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="e79c7-122">enforceSignatureCheck</span></span>|<span data-ttu-id="e79c7-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="e79c7-123">Boolean</span></span>|<span data-ttu-id="e79c7-124">Um valor que indica se uma verificação de assinatura é imposta.</span><span class="sxs-lookup"><span data-stu-id="e79c7-124">A value indicating whether a signature check is enforced.</span></span>|
|<span data-ttu-id="e79c7-125">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="e79c7-125">runAs32Bit</span></span>|<span data-ttu-id="e79c7-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="e79c7-126">Boolean</span></span>|<span data-ttu-id="e79c7-127">Um valor que indica se o script deve ser executado como 32 bits.</span><span class="sxs-lookup"><span data-stu-id="e79c7-127">A value indicating whether the script should run as 32-bit.</span></span>|
|<span data-ttu-id="e79c7-128">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="e79c7-128">runAsAccount</span></span>|[<span data-ttu-id="e79c7-129">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="e79c7-129">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="e79c7-130">O contexto de execução do script.</span><span class="sxs-lookup"><span data-stu-id="e79c7-130">The execution context of the script.</span></span> <span data-ttu-id="e79c7-131">Não especifique esse valor se a regra for usada para detecção.</span><span class="sxs-lookup"><span data-stu-id="e79c7-131">Do not specify this value if the rule is used for detection.</span></span> <span data-ttu-id="e79c7-132">As regras de detecção de script serão executadas no mesmo contexto do contexto de instalação de aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="e79c7-132">Script detection rules will run in the same context as the associated app install context.</span></span> <span data-ttu-id="e79c7-133">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="e79c7-133">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="e79c7-134">scriptContent</span><span class="sxs-lookup"><span data-stu-id="e79c7-134">scriptContent</span></span>|<span data-ttu-id="e79c7-135">String</span><span class="sxs-lookup"><span data-stu-id="e79c7-135">String</span></span>|<span data-ttu-id="e79c7-136">O conteúdo de script codificado em base64.</span><span class="sxs-lookup"><span data-stu-id="e79c7-136">The base64-encoded script content.</span></span>|
|<span data-ttu-id="e79c7-137">OperationType</span><span class="sxs-lookup"><span data-stu-id="e79c7-137">operationType</span></span>|[<span data-ttu-id="e79c7-138">win32LobAppPowerShellScriptRuleOperationType</span><span class="sxs-lookup"><span data-stu-id="e79c7-138">win32LobAppPowerShellScriptRuleOperationType</span></span>](../resources/intune-apps-win32lobapppowershellscriptruleoperationtype.md)|<span data-ttu-id="e79c7-139">O tipo de operação de comparação de saída de script.</span><span class="sxs-lookup"><span data-stu-id="e79c7-139">The script output comparison operation type.</span></span> <span data-ttu-id="e79c7-140">Use não configurado (o valor padrão) se a regra for usada para detecção.</span><span class="sxs-lookup"><span data-stu-id="e79c7-140">Use NotConfigured (the default value) if the rule is used for detection.</span></span> <span data-ttu-id="e79c7-141">Os valores possíveis são: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span><span class="sxs-lookup"><span data-stu-id="e79c7-141">Possible values are: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span></span>|
|<span data-ttu-id="e79c7-142">operator</span><span class="sxs-lookup"><span data-stu-id="e79c7-142">operator</span></span>|[<span data-ttu-id="e79c7-143">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="e79c7-143">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="e79c7-144">O operador de saída de script.</span><span class="sxs-lookup"><span data-stu-id="e79c7-144">The script output operator.</span></span> <span data-ttu-id="e79c7-145">Use não configurado (o valor padrão) se a regra for usada para detecção.</span><span class="sxs-lookup"><span data-stu-id="e79c7-145">Use NotConfigured (the default value) if the rule is used for detection.</span></span> <span data-ttu-id="e79c7-146">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="e79c7-146">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="e79c7-147">ComparisonValue</span><span class="sxs-lookup"><span data-stu-id="e79c7-147">comparisonValue</span></span>|<span data-ttu-id="e79c7-148">String</span><span class="sxs-lookup"><span data-stu-id="e79c7-148">String</span></span>|<span data-ttu-id="e79c7-149">O valor de comparação de saída do script.</span><span class="sxs-lookup"><span data-stu-id="e79c7-149">The script output comparison value.</span></span> <span data-ttu-id="e79c7-150">Não especifique um valor se a regra for usada para detecção.</span><span class="sxs-lookup"><span data-stu-id="e79c7-150">Do not specify a value if the rule is used for detection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e79c7-151">Relações</span><span class="sxs-lookup"><span data-stu-id="e79c7-151">Relationships</span></span>
<span data-ttu-id="e79c7-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e79c7-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e79c7-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e79c7-153">JSON Representation</span></span>
<span data-ttu-id="e79c7-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e79c7-154">Here is a JSON representation of the resource.</span></span>
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





