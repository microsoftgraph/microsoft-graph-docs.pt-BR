---
title: tipo de recurso win32LobAppRegistryRule
description: Um tipo complexo para armazenar dados de regra de registro para um aplicativo LOB Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 64343873093428849462cbdc12fc078a7a028e2d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080035"
---
# <a name="win32lobappregistryrule-resource-type"></a><span data-ttu-id="64167-103">tipo de recurso win32LobAppRegistryRule</span><span class="sxs-lookup"><span data-stu-id="64167-103">win32LobAppRegistryRule resource type</span></span>

<span data-ttu-id="64167-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64167-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64167-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="64167-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64167-106">Um tipo complexo para armazenar dados de regra de registro para um aplicativo LOB Win32.</span><span class="sxs-lookup"><span data-stu-id="64167-106">A complex type to store registry rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="64167-107">Herda de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="64167-107">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="64167-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="64167-108">Properties</span></span>
|<span data-ttu-id="64167-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64167-109">Property</span></span>|<span data-ttu-id="64167-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="64167-110">Type</span></span>|<span data-ttu-id="64167-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="64167-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64167-112">ruleType</span><span class="sxs-lookup"><span data-stu-id="64167-112">ruleType</span></span>|[<span data-ttu-id="64167-113">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="64167-113">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="64167-114">O tipo de regra que indica o objetivo da regra.</span><span class="sxs-lookup"><span data-stu-id="64167-114">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="64167-115">Herdado de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="64167-115">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="64167-116">Os valores possíveis são: `detection` e `requirement`.</span><span class="sxs-lookup"><span data-stu-id="64167-116">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="64167-117">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="64167-117">check32BitOn64System</span></span>|<span data-ttu-id="64167-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="64167-118">Boolean</span></span>|<span data-ttu-id="64167-119">Um valor que indica se é para pesquisar o registro de 32 bits em sistemas de 64 bits.</span><span class="sxs-lookup"><span data-stu-id="64167-119">A value indicating whether to search the 32-bit registry on 64-bit systems.</span></span>|
|<span data-ttu-id="64167-120">Caminho-chave</span><span class="sxs-lookup"><span data-stu-id="64167-120">keyPath</span></span>|<span data-ttu-id="64167-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64167-121">String</span></span>|<span data-ttu-id="64167-122">O caminho completo da entrada de registro que contém o valor a ser detectado.</span><span class="sxs-lookup"><span data-stu-id="64167-122">The full path of the registry entry containing the value to detect.</span></span>|
|<span data-ttu-id="64167-123">valueName</span><span class="sxs-lookup"><span data-stu-id="64167-123">valueName</span></span>|<span data-ttu-id="64167-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64167-124">String</span></span>|<span data-ttu-id="64167-125">O nome do valor do registro a ser detectado.</span><span class="sxs-lookup"><span data-stu-id="64167-125">The name of the registry value to detect.</span></span>|
|<span data-ttu-id="64167-126">OperationType</span><span class="sxs-lookup"><span data-stu-id="64167-126">operationType</span></span>|[<span data-ttu-id="64167-127">win32LobAppRegistryRuleOperationType</span><span class="sxs-lookup"><span data-stu-id="64167-127">win32LobAppRegistryRuleOperationType</span></span>](../resources/intune-apps-win32lobappregistryruleoperationtype.md)|<span data-ttu-id="64167-128">O tipo de operação do registro.</span><span class="sxs-lookup"><span data-stu-id="64167-128">The registry operation type.</span></span> <span data-ttu-id="64167-129">Os possíveis valores são: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="64167-129">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="64167-130">operator</span><span class="sxs-lookup"><span data-stu-id="64167-130">operator</span></span>|[<span data-ttu-id="64167-131">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="64167-131">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="64167-132">O operador para detecção de registro.</span><span class="sxs-lookup"><span data-stu-id="64167-132">The operator for registry detection.</span></span> <span data-ttu-id="64167-133">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="64167-133">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="64167-134">ComparisonValue</span><span class="sxs-lookup"><span data-stu-id="64167-134">comparisonValue</span></span>|<span data-ttu-id="64167-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64167-135">String</span></span>|<span data-ttu-id="64167-136">O valor de comparação do registro.</span><span class="sxs-lookup"><span data-stu-id="64167-136">The registry comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64167-137">Relações</span><span class="sxs-lookup"><span data-stu-id="64167-137">Relationships</span></span>
<span data-ttu-id="64167-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="64167-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="64167-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="64167-139">JSON Representation</span></span>
<span data-ttu-id="64167-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="64167-140">Here is a JSON representation of the resource.</span></span>
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





