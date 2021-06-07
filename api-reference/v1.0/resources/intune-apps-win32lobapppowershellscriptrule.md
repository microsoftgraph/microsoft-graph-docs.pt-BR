---
title: Tipo de recurso win32LobAppPowerShellScriptRule
description: Um tipo complexo para armazenar os dados da regra de script do PowerShell para um aplicativo LOB win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dcc9afa8f58462bda69c96990e37529667d20445
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758985"
---
# <a name="win32lobapppowershellscriptrule-resource-type"></a><span data-ttu-id="45b3f-103">Tipo de recurso win32LobAppPowerShellScriptRule</span><span class="sxs-lookup"><span data-stu-id="45b3f-103">win32LobAppPowerShellScriptRule resource type</span></span>

<span data-ttu-id="45b3f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45b3f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45b3f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45b3f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45b3f-106">Um tipo complexo para armazenar os dados da regra de script do PowerShell para um aplicativo LOB win32.</span><span class="sxs-lookup"><span data-stu-id="45b3f-106">A complex type to store the PowerShell script rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="45b3f-107">Herda de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="45b3f-107">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="45b3f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="45b3f-108">Properties</span></span>
|<span data-ttu-id="45b3f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45b3f-109">Property</span></span>|<span data-ttu-id="45b3f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="45b3f-110">Type</span></span>|<span data-ttu-id="45b3f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="45b3f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45b3f-112">ruleType</span><span class="sxs-lookup"><span data-stu-id="45b3f-112">ruleType</span></span>|[<span data-ttu-id="45b3f-113">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="45b3f-113">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="45b3f-114">O tipo de regra que indica a finalidade da regra.</span><span class="sxs-lookup"><span data-stu-id="45b3f-114">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="45b3f-115">Herdado [de win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="45b3f-115">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="45b3f-116">Os valores possíveis são: `detection` e `requirement`.</span><span class="sxs-lookup"><span data-stu-id="45b3f-116">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="45b3f-117">displayName</span><span class="sxs-lookup"><span data-stu-id="45b3f-117">displayName</span></span>|<span data-ttu-id="45b3f-118">String</span><span class="sxs-lookup"><span data-stu-id="45b3f-118">String</span></span>|<span data-ttu-id="45b3f-119">O nome de exibição da regra.</span><span class="sxs-lookup"><span data-stu-id="45b3f-119">The display name for the rule.</span></span> <span data-ttu-id="45b3f-120">Não especifique esse valor se a regra for usada para detecção.</span><span class="sxs-lookup"><span data-stu-id="45b3f-120">Do not specify this value if the rule is used for detection.</span></span>|
|<span data-ttu-id="45b3f-121">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="45b3f-121">enforceSignatureCheck</span></span>|<span data-ttu-id="45b3f-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="45b3f-122">Boolean</span></span>|<span data-ttu-id="45b3f-123">Um valor que indica se uma verificação de assinatura é imposta.</span><span class="sxs-lookup"><span data-stu-id="45b3f-123">A value indicating whether a signature check is enforced.</span></span>|
|<span data-ttu-id="45b3f-124">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="45b3f-124">runAs32Bit</span></span>|<span data-ttu-id="45b3f-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="45b3f-125">Boolean</span></span>|<span data-ttu-id="45b3f-126">Um valor que indica se o script deve ser executado como 32 bits.</span><span class="sxs-lookup"><span data-stu-id="45b3f-126">A value indicating whether the script should run as 32-bit.</span></span>|
|<span data-ttu-id="45b3f-127">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="45b3f-127">runAsAccount</span></span>|[<span data-ttu-id="45b3f-128">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="45b3f-128">runAsAccountType</span></span>](../resources/intune-apps-runasaccounttype.md)|<span data-ttu-id="45b3f-129">O contexto de execução do script.</span><span class="sxs-lookup"><span data-stu-id="45b3f-129">The execution context of the script.</span></span> <span data-ttu-id="45b3f-130">Não especifique esse valor se a regra for usada para detecção.</span><span class="sxs-lookup"><span data-stu-id="45b3f-130">Do not specify this value if the rule is used for detection.</span></span> <span data-ttu-id="45b3f-131">As regras de detecção de script serão executados no mesmo contexto que o contexto de instalação do aplicativo associado.</span><span class="sxs-lookup"><span data-stu-id="45b3f-131">Script detection rules will run in the same context as the associated app install context.</span></span> <span data-ttu-id="45b3f-132">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="45b3f-132">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="45b3f-133">scriptContent</span><span class="sxs-lookup"><span data-stu-id="45b3f-133">scriptContent</span></span>|<span data-ttu-id="45b3f-134">String</span><span class="sxs-lookup"><span data-stu-id="45b3f-134">String</span></span>|<span data-ttu-id="45b3f-135">O conteúdo de script codificado com base64.</span><span class="sxs-lookup"><span data-stu-id="45b3f-135">The base64-encoded script content.</span></span>|
|<span data-ttu-id="45b3f-136">operationType</span><span class="sxs-lookup"><span data-stu-id="45b3f-136">operationType</span></span>|[<span data-ttu-id="45b3f-137">win32LobAppPowerShellScriptRuleOperationType</span><span class="sxs-lookup"><span data-stu-id="45b3f-137">win32LobAppPowerShellScriptRuleOperationType</span></span>](../resources/intune-apps-win32lobapppowershellscriptruleoperationtype.md)|<span data-ttu-id="45b3f-138">O tipo de operação de comparação de saída de script.</span><span class="sxs-lookup"><span data-stu-id="45b3f-138">The script output comparison operation type.</span></span> <span data-ttu-id="45b3f-139">Use NotConfigured (o valor padrão) se a regra for usada para detecção.</span><span class="sxs-lookup"><span data-stu-id="45b3f-139">Use NotConfigured (the default value) if the rule is used for detection.</span></span> <span data-ttu-id="45b3f-140">Os valores possíveis são: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span><span class="sxs-lookup"><span data-stu-id="45b3f-140">Possible values are: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span></span>|
|<span data-ttu-id="45b3f-141">operator</span><span class="sxs-lookup"><span data-stu-id="45b3f-141">operator</span></span>|[<span data-ttu-id="45b3f-142">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="45b3f-142">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="45b3f-143">O operador de saída de script.</span><span class="sxs-lookup"><span data-stu-id="45b3f-143">The script output operator.</span></span> <span data-ttu-id="45b3f-144">Use NotConfigured (o valor padrão) se a regra for usada para detecção.</span><span class="sxs-lookup"><span data-stu-id="45b3f-144">Use NotConfigured (the default value) if the rule is used for detection.</span></span> <span data-ttu-id="45b3f-145">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="45b3f-145">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="45b3f-146">comparisonValue</span><span class="sxs-lookup"><span data-stu-id="45b3f-146">comparisonValue</span></span>|<span data-ttu-id="45b3f-147">String</span><span class="sxs-lookup"><span data-stu-id="45b3f-147">String</span></span>|<span data-ttu-id="45b3f-148">O valor de comparação de saída de script.</span><span class="sxs-lookup"><span data-stu-id="45b3f-148">The script output comparison value.</span></span> <span data-ttu-id="45b3f-149">Não especifique um valor se a regra for usada para detecção.</span><span class="sxs-lookup"><span data-stu-id="45b3f-149">Do not specify a value if the rule is used for detection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45b3f-150">Relações</span><span class="sxs-lookup"><span data-stu-id="45b3f-150">Relationships</span></span>
<span data-ttu-id="45b3f-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="45b3f-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="45b3f-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="45b3f-152">JSON Representation</span></span>
<span data-ttu-id="45b3f-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="45b3f-153">Here is a JSON representation of the resource.</span></span>
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




