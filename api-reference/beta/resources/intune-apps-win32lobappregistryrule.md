---
title: tipo de recurso win32LobAppRegistryRule
description: Um tipo complexo para armazenar dados de regra de registro para um aplicativo LOB Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d39d8e2881d20d58348e9a2c25b2b808c40b9fe5
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49217084"
---
# <a name="win32lobappregistryrule-resource-type"></a><span data-ttu-id="9d777-103">tipo de recurso win32LobAppRegistryRule</span><span class="sxs-lookup"><span data-stu-id="9d777-103">win32LobAppRegistryRule resource type</span></span>

<span data-ttu-id="9d777-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d777-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d777-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9d777-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d777-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9d777-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d777-107">Um tipo complexo para armazenar dados de regra de registro para um aplicativo LOB Win32.</span><span class="sxs-lookup"><span data-stu-id="9d777-107">A complex type to store registry rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="9d777-108">Herda de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="9d777-108">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9d777-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d777-109">Properties</span></span>
|<span data-ttu-id="9d777-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d777-110">Property</span></span>|<span data-ttu-id="9d777-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d777-111">Type</span></span>|<span data-ttu-id="9d777-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d777-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d777-113">ruleType</span><span class="sxs-lookup"><span data-stu-id="9d777-113">ruleType</span></span>|[<span data-ttu-id="9d777-114">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="9d777-114">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="9d777-115">O tipo de regra que indica o objetivo da regra.</span><span class="sxs-lookup"><span data-stu-id="9d777-115">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="9d777-116">Herdado de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="9d777-116">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="9d777-117">Os valores possíveis são: `detection` e `requirement`.</span><span class="sxs-lookup"><span data-stu-id="9d777-117">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="9d777-118">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="9d777-118">check32BitOn64System</span></span>|<span data-ttu-id="9d777-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="9d777-119">Boolean</span></span>|<span data-ttu-id="9d777-120">Um valor que indica se é para pesquisar o registro de 32 bits em sistemas de 64 bits.</span><span class="sxs-lookup"><span data-stu-id="9d777-120">A value indicating whether to search the 32-bit registry on 64-bit systems.</span></span>|
|<span data-ttu-id="9d777-121">Caminho-chave</span><span class="sxs-lookup"><span data-stu-id="9d777-121">keyPath</span></span>|<span data-ttu-id="9d777-122">String</span><span class="sxs-lookup"><span data-stu-id="9d777-122">String</span></span>|<span data-ttu-id="9d777-123">O caminho completo da entrada de registro que contém o valor a ser detectado.</span><span class="sxs-lookup"><span data-stu-id="9d777-123">The full path of the registry entry containing the value to detect.</span></span>|
|<span data-ttu-id="9d777-124">valueName</span><span class="sxs-lookup"><span data-stu-id="9d777-124">valueName</span></span>|<span data-ttu-id="9d777-125">String</span><span class="sxs-lookup"><span data-stu-id="9d777-125">String</span></span>|<span data-ttu-id="9d777-126">O nome do valor do registro a ser detectado.</span><span class="sxs-lookup"><span data-stu-id="9d777-126">The name of the registry value to detect.</span></span>|
|<span data-ttu-id="9d777-127">OperationType</span><span class="sxs-lookup"><span data-stu-id="9d777-127">operationType</span></span>|[<span data-ttu-id="9d777-128">win32LobAppRegistryRuleOperationType</span><span class="sxs-lookup"><span data-stu-id="9d777-128">win32LobAppRegistryRuleOperationType</span></span>](../resources/intune-apps-win32lobappregistryruleoperationtype.md)|<span data-ttu-id="9d777-129">O tipo de operação do registro.</span><span class="sxs-lookup"><span data-stu-id="9d777-129">The registry operation type.</span></span> <span data-ttu-id="9d777-130">Os possíveis valores são: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="9d777-130">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="9d777-131">operator</span><span class="sxs-lookup"><span data-stu-id="9d777-131">operator</span></span>|[<span data-ttu-id="9d777-132">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="9d777-132">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="9d777-133">O operador para detecção de registro.</span><span class="sxs-lookup"><span data-stu-id="9d777-133">The operator for registry detection.</span></span> <span data-ttu-id="9d777-134">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="9d777-134">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="9d777-135">ComparisonValue</span><span class="sxs-lookup"><span data-stu-id="9d777-135">comparisonValue</span></span>|<span data-ttu-id="9d777-136">String</span><span class="sxs-lookup"><span data-stu-id="9d777-136">String</span></span>|<span data-ttu-id="9d777-137">O valor de comparação do registro.</span><span class="sxs-lookup"><span data-stu-id="9d777-137">The registry comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d777-138">Relações</span><span class="sxs-lookup"><span data-stu-id="9d777-138">Relationships</span></span>
<span data-ttu-id="9d777-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9d777-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d777-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d777-140">JSON Representation</span></span>
<span data-ttu-id="9d777-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9d777-141">Here is a JSON representation of the resource.</span></span>
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




