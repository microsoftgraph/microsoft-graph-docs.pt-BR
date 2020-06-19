---
title: tipo de recurso win32LobAppFileSystemRule
description: Um tipo complexo para armazenar dados de regra de arquivo ou pasta para um aplicativo LOB Win32.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fa01642dd36cd8dc79f713446df05a9559294f56
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790828"
---
# <a name="win32lobappfilesystemrule-resource-type"></a><span data-ttu-id="9b35b-103">tipo de recurso win32LobAppFileSystemRule</span><span class="sxs-lookup"><span data-stu-id="9b35b-103">win32LobAppFileSystemRule resource type</span></span>

<span data-ttu-id="9b35b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b35b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b35b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9b35b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b35b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9b35b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b35b-107">Um tipo complexo para armazenar dados de regra de arquivo ou pasta para um aplicativo LOB Win32.</span><span class="sxs-lookup"><span data-stu-id="9b35b-107">A complex type to store file or folder rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="9b35b-108">Herda de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="9b35b-108">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9b35b-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9b35b-109">Properties</span></span>
|<span data-ttu-id="9b35b-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b35b-110">Property</span></span>|<span data-ttu-id="9b35b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b35b-111">Type</span></span>|<span data-ttu-id="9b35b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b35b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b35b-113">ruleType</span><span class="sxs-lookup"><span data-stu-id="9b35b-113">ruleType</span></span>|[<span data-ttu-id="9b35b-114">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="9b35b-114">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="9b35b-115">O tipo de regra que indica o objetivo da regra.</span><span class="sxs-lookup"><span data-stu-id="9b35b-115">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="9b35b-116">Herdado de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="9b35b-116">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="9b35b-117">Os valores possíveis são: `detection` e `requirement`.</span><span class="sxs-lookup"><span data-stu-id="9b35b-117">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="9b35b-118">caminho</span><span class="sxs-lookup"><span data-stu-id="9b35b-118">path</span></span>|<span data-ttu-id="9b35b-119">String</span><span class="sxs-lookup"><span data-stu-id="9b35b-119">String</span></span>|<span data-ttu-id="9b35b-120">O caminho do arquivo ou da pasta a ser pesquisado.</span><span class="sxs-lookup"><span data-stu-id="9b35b-120">The file or folder path to look up.</span></span>|
|<span data-ttu-id="9b35b-121">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="9b35b-121">fileOrFolderName</span></span>|<span data-ttu-id="9b35b-122">String</span><span class="sxs-lookup"><span data-stu-id="9b35b-122">String</span></span>|<span data-ttu-id="9b35b-123">O nome do arquivo ou pasta a ser procurado.</span><span class="sxs-lookup"><span data-stu-id="9b35b-123">The file or folder name to look up.</span></span>|
|<span data-ttu-id="9b35b-124">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="9b35b-124">check32BitOn64System</span></span>|<span data-ttu-id="9b35b-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b35b-125">Boolean</span></span>|<span data-ttu-id="9b35b-126">Um valor que indica se as variáveis de ambiente serão expandidas no contexto de 32 bits em sistemas de 64 bits.</span><span class="sxs-lookup"><span data-stu-id="9b35b-126">A value indicating whether to expand environment variables in the 32-bit context on 64-bit systems.</span></span>|
|<span data-ttu-id="9b35b-127">OperationType</span><span class="sxs-lookup"><span data-stu-id="9b35b-127">operationType</span></span>|[<span data-ttu-id="9b35b-128">win32LobAppFileSystemOperationType</span><span class="sxs-lookup"><span data-stu-id="9b35b-128">win32LobAppFileSystemOperationType</span></span>](../resources/intune-apps-win32lobappfilesystemoperationtype.md)|<span data-ttu-id="9b35b-129">O tipo de operação do sistema de arquivos.</span><span class="sxs-lookup"><span data-stu-id="9b35b-129">The file system operation type.</span></span> <span data-ttu-id="9b35b-130">Os valores possíveis são: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span><span class="sxs-lookup"><span data-stu-id="9b35b-130">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|
|<span data-ttu-id="9b35b-131">operator</span><span class="sxs-lookup"><span data-stu-id="9b35b-131">operator</span></span>|[<span data-ttu-id="9b35b-132">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="9b35b-132">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="9b35b-133">O operador para detecção de arquivo ou pasta.</span><span class="sxs-lookup"><span data-stu-id="9b35b-133">The operator for file or folder detection.</span></span> <span data-ttu-id="9b35b-134">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="9b35b-134">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="9b35b-135">ComparisonValue</span><span class="sxs-lookup"><span data-stu-id="9b35b-135">comparisonValue</span></span>|<span data-ttu-id="9b35b-136">String</span><span class="sxs-lookup"><span data-stu-id="9b35b-136">String</span></span>|<span data-ttu-id="9b35b-137">O valor de comparação de arquivo ou pasta.</span><span class="sxs-lookup"><span data-stu-id="9b35b-137">The file or folder comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b35b-138">Relações</span><span class="sxs-lookup"><span data-stu-id="9b35b-138">Relationships</span></span>
<span data-ttu-id="9b35b-139">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="9b35b-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b35b-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9b35b-140">JSON Representation</span></span>
<span data-ttu-id="9b35b-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9b35b-141">Here is a JSON representation of the resource.</span></span>
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



