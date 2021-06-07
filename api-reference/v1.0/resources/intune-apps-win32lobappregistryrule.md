---
title: Tipo de recurso win32LobAppRegistryRule
description: Um tipo complexo para armazenar dados de regra do Registro para um aplicativo LOB win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bfa6ed9e95a86abe1d87646a7c57f953be539f69
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758978"
---
# <a name="win32lobappregistryrule-resource-type"></a><span data-ttu-id="033f6-103">Tipo de recurso win32LobAppRegistryRule</span><span class="sxs-lookup"><span data-stu-id="033f6-103">win32LobAppRegistryRule resource type</span></span>

<span data-ttu-id="033f6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="033f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="033f6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="033f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="033f6-106">Um tipo complexo para armazenar dados de regra do Registro para um aplicativo LOB win32.</span><span class="sxs-lookup"><span data-stu-id="033f6-106">A complex type to store registry rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="033f6-107">Herda de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="033f6-107">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="033f6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="033f6-108">Properties</span></span>
|<span data-ttu-id="033f6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="033f6-109">Property</span></span>|<span data-ttu-id="033f6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="033f6-110">Type</span></span>|<span data-ttu-id="033f6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="033f6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="033f6-112">ruleType</span><span class="sxs-lookup"><span data-stu-id="033f6-112">ruleType</span></span>|[<span data-ttu-id="033f6-113">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="033f6-113">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="033f6-114">O tipo de regra que indica a finalidade da regra.</span><span class="sxs-lookup"><span data-stu-id="033f6-114">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="033f6-115">Herdado [de win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="033f6-115">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="033f6-116">Os valores possíveis são: `detection` e `requirement`.</span><span class="sxs-lookup"><span data-stu-id="033f6-116">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="033f6-117">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="033f6-117">check32BitOn64System</span></span>|<span data-ttu-id="033f6-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="033f6-118">Boolean</span></span>|<span data-ttu-id="033f6-119">Um valor que indica se o registro de 32 bits deve ser pesquisado em sistemas de 64 bits.</span><span class="sxs-lookup"><span data-stu-id="033f6-119">A value indicating whether to search the 32-bit registry on 64-bit systems.</span></span>|
|<span data-ttu-id="033f6-120">keyPath</span><span class="sxs-lookup"><span data-stu-id="033f6-120">keyPath</span></span>|<span data-ttu-id="033f6-121">String</span><span class="sxs-lookup"><span data-stu-id="033f6-121">String</span></span>|<span data-ttu-id="033f6-122">O caminho completo da entrada do Registro contendo o valor a ser detectado.</span><span class="sxs-lookup"><span data-stu-id="033f6-122">The full path of the registry entry containing the value to detect.</span></span>|
|<span data-ttu-id="033f6-123">valueName</span><span class="sxs-lookup"><span data-stu-id="033f6-123">valueName</span></span>|<span data-ttu-id="033f6-124">String</span><span class="sxs-lookup"><span data-stu-id="033f6-124">String</span></span>|<span data-ttu-id="033f6-125">O nome do valor do Registro a ser detectado.</span><span class="sxs-lookup"><span data-stu-id="033f6-125">The name of the registry value to detect.</span></span>|
|<span data-ttu-id="033f6-126">operationType</span><span class="sxs-lookup"><span data-stu-id="033f6-126">operationType</span></span>|[<span data-ttu-id="033f6-127">win32LobAppRegistryRuleOperationType</span><span class="sxs-lookup"><span data-stu-id="033f6-127">win32LobAppRegistryRuleOperationType</span></span>](../resources/intune-apps-win32lobappregistryruleoperationtype.md)|<span data-ttu-id="033f6-128">O tipo de operação do Registro.</span><span class="sxs-lookup"><span data-stu-id="033f6-128">The registry operation type.</span></span> <span data-ttu-id="033f6-129">Os possíveis valores são: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="033f6-129">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="033f6-130">operator</span><span class="sxs-lookup"><span data-stu-id="033f6-130">operator</span></span>|[<span data-ttu-id="033f6-131">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="033f6-131">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="033f6-132">O operador para detecção do Registro.</span><span class="sxs-lookup"><span data-stu-id="033f6-132">The operator for registry detection.</span></span> <span data-ttu-id="033f6-133">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="033f6-133">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="033f6-134">comparisonValue</span><span class="sxs-lookup"><span data-stu-id="033f6-134">comparisonValue</span></span>|<span data-ttu-id="033f6-135">String</span><span class="sxs-lookup"><span data-stu-id="033f6-135">String</span></span>|<span data-ttu-id="033f6-136">O valor de comparação do Registro.</span><span class="sxs-lookup"><span data-stu-id="033f6-136">The registry comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="033f6-137">Relações</span><span class="sxs-lookup"><span data-stu-id="033f6-137">Relationships</span></span>
<span data-ttu-id="033f6-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="033f6-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="033f6-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="033f6-139">JSON Representation</span></span>
<span data-ttu-id="033f6-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="033f6-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRegistryRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRegistryRule",
  "ruleType": "String",
  "check32BitOn64System": true,
  "keyPath": "String",
  "valueName": "String",
  "operationType": "String",
  "operator": "String",
  "comparisonValue": "String"
}
```




