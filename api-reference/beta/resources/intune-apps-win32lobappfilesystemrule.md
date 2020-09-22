---
title: tipo de recurso win32LobAppFileSystemRule
description: Um tipo complexo para armazenar dados de regra de arquivo ou pasta para um aplicativo LOB Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c83fa4bf5f3d24a4b171a8492f4212720242acdf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033780"
---
# <a name="win32lobappfilesystemrule-resource-type"></a><span data-ttu-id="e7540-103">tipo de recurso win32LobAppFileSystemRule</span><span class="sxs-lookup"><span data-stu-id="e7540-103">win32LobAppFileSystemRule resource type</span></span>

<span data-ttu-id="e7540-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7540-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7540-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e7540-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7540-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e7540-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7540-107">Um tipo complexo para armazenar dados de regra de arquivo ou pasta para um aplicativo LOB Win32.</span><span class="sxs-lookup"><span data-stu-id="e7540-107">A complex type to store file or folder rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="e7540-108">Herda de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="e7540-108">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e7540-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e7540-109">Properties</span></span>
|<span data-ttu-id="e7540-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e7540-110">Property</span></span>|<span data-ttu-id="e7540-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7540-111">Type</span></span>|<span data-ttu-id="e7540-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7540-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7540-113">ruleType</span><span class="sxs-lookup"><span data-stu-id="e7540-113">ruleType</span></span>|[<span data-ttu-id="e7540-114">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="e7540-114">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="e7540-115">O tipo de regra que indica o objetivo da regra.</span><span class="sxs-lookup"><span data-stu-id="e7540-115">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="e7540-116">Herdado de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="e7540-116">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="e7540-117">Os valores possíveis são: `detection` e `requirement`.</span><span class="sxs-lookup"><span data-stu-id="e7540-117">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="e7540-118">caminho</span><span class="sxs-lookup"><span data-stu-id="e7540-118">path</span></span>|<span data-ttu-id="e7540-119">String</span><span class="sxs-lookup"><span data-stu-id="e7540-119">String</span></span>|<span data-ttu-id="e7540-120">O caminho do arquivo ou da pasta a ser pesquisado.</span><span class="sxs-lookup"><span data-stu-id="e7540-120">The file or folder path to look up.</span></span>|
|<span data-ttu-id="e7540-121">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="e7540-121">fileOrFolderName</span></span>|<span data-ttu-id="e7540-122">String</span><span class="sxs-lookup"><span data-stu-id="e7540-122">String</span></span>|<span data-ttu-id="e7540-123">O nome do arquivo ou pasta a ser procurado.</span><span class="sxs-lookup"><span data-stu-id="e7540-123">The file or folder name to look up.</span></span>|
|<span data-ttu-id="e7540-124">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="e7540-124">check32BitOn64System</span></span>|<span data-ttu-id="e7540-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="e7540-125">Boolean</span></span>|<span data-ttu-id="e7540-126">Um valor que indica se as variáveis de ambiente serão expandidas no contexto de 32 bits em sistemas de 64 bits.</span><span class="sxs-lookup"><span data-stu-id="e7540-126">A value indicating whether to expand environment variables in the 32-bit context on 64-bit systems.</span></span>|
|<span data-ttu-id="e7540-127">OperationType</span><span class="sxs-lookup"><span data-stu-id="e7540-127">operationType</span></span>|[<span data-ttu-id="e7540-128">win32LobAppFileSystemOperationType</span><span class="sxs-lookup"><span data-stu-id="e7540-128">win32LobAppFileSystemOperationType</span></span>](../resources/intune-apps-win32lobappfilesystemoperationtype.md)|<span data-ttu-id="e7540-129">O tipo de operação do sistema de arquivos.</span><span class="sxs-lookup"><span data-stu-id="e7540-129">The file system operation type.</span></span> <span data-ttu-id="e7540-130">Os valores possíveis são: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span><span class="sxs-lookup"><span data-stu-id="e7540-130">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|
|<span data-ttu-id="e7540-131">operator</span><span class="sxs-lookup"><span data-stu-id="e7540-131">operator</span></span>|[<span data-ttu-id="e7540-132">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="e7540-132">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="e7540-133">O operador para detecção de arquivo ou pasta.</span><span class="sxs-lookup"><span data-stu-id="e7540-133">The operator for file or folder detection.</span></span> <span data-ttu-id="e7540-134">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="e7540-134">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="e7540-135">ComparisonValue</span><span class="sxs-lookup"><span data-stu-id="e7540-135">comparisonValue</span></span>|<span data-ttu-id="e7540-136">String</span><span class="sxs-lookup"><span data-stu-id="e7540-136">String</span></span>|<span data-ttu-id="e7540-137">O valor de comparação de arquivo ou pasta.</span><span class="sxs-lookup"><span data-stu-id="e7540-137">The file or folder comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7540-138">Relações</span><span class="sxs-lookup"><span data-stu-id="e7540-138">Relationships</span></span>
<span data-ttu-id="e7540-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e7540-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7540-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e7540-140">JSON Representation</span></span>
<span data-ttu-id="e7540-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e7540-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemRule",
  "ruleType": "String",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": true,
  "operationType": "String",
  "operator": "String",
  "comparisonValue": "String"
}
```






