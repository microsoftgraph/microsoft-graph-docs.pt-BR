---
title: tipo de recurso win32LobAppFileSystemRule
description: Um tipo complexo para armazenar dados de regra de arquivo ou pasta para um aplicativo LOB Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9e3873b85256f1c79c0102e1f410619d98c51594
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080051"
---
# <a name="win32lobappfilesystemrule-resource-type"></a><span data-ttu-id="1130f-103">tipo de recurso win32LobAppFileSystemRule</span><span class="sxs-lookup"><span data-stu-id="1130f-103">win32LobAppFileSystemRule resource type</span></span>

<span data-ttu-id="1130f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1130f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1130f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1130f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1130f-106">Um tipo complexo para armazenar dados de regra de arquivo ou pasta para um aplicativo LOB Win32.</span><span class="sxs-lookup"><span data-stu-id="1130f-106">A complex type to store file or folder rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="1130f-107">Herda de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="1130f-107">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1130f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1130f-108">Properties</span></span>
|<span data-ttu-id="1130f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1130f-109">Property</span></span>|<span data-ttu-id="1130f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1130f-110">Type</span></span>|<span data-ttu-id="1130f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1130f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1130f-112">ruleType</span><span class="sxs-lookup"><span data-stu-id="1130f-112">ruleType</span></span>|[<span data-ttu-id="1130f-113">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="1130f-113">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="1130f-114">O tipo de regra que indica o objetivo da regra.</span><span class="sxs-lookup"><span data-stu-id="1130f-114">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="1130f-115">Herdado de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="1130f-115">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="1130f-116">Os valores possíveis são: `detection` e `requirement`.</span><span class="sxs-lookup"><span data-stu-id="1130f-116">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="1130f-117">caminho</span><span class="sxs-lookup"><span data-stu-id="1130f-117">path</span></span>|<span data-ttu-id="1130f-118">String</span><span class="sxs-lookup"><span data-stu-id="1130f-118">String</span></span>|<span data-ttu-id="1130f-119">O caminho do arquivo ou da pasta a ser pesquisado.</span><span class="sxs-lookup"><span data-stu-id="1130f-119">The file or folder path to look up.</span></span>|
|<span data-ttu-id="1130f-120">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="1130f-120">fileOrFolderName</span></span>|<span data-ttu-id="1130f-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1130f-121">String</span></span>|<span data-ttu-id="1130f-122">O nome do arquivo ou pasta a ser procurado.</span><span class="sxs-lookup"><span data-stu-id="1130f-122">The file or folder name to look up.</span></span>|
|<span data-ttu-id="1130f-123">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="1130f-123">check32BitOn64System</span></span>|<span data-ttu-id="1130f-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="1130f-124">Boolean</span></span>|<span data-ttu-id="1130f-125">Um valor que indica se as variáveis de ambiente serão expandidas no contexto de 32 bits em sistemas de 64 bits.</span><span class="sxs-lookup"><span data-stu-id="1130f-125">A value indicating whether to expand environment variables in the 32-bit context on 64-bit systems.</span></span>|
|<span data-ttu-id="1130f-126">OperationType</span><span class="sxs-lookup"><span data-stu-id="1130f-126">operationType</span></span>|[<span data-ttu-id="1130f-127">win32LobAppFileSystemOperationType</span><span class="sxs-lookup"><span data-stu-id="1130f-127">win32LobAppFileSystemOperationType</span></span>](../resources/intune-apps-win32lobappfilesystemoperationtype.md)|<span data-ttu-id="1130f-128">O tipo de operação do sistema de arquivos.</span><span class="sxs-lookup"><span data-stu-id="1130f-128">The file system operation type.</span></span> <span data-ttu-id="1130f-129">Os possíveis valores são: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.</span><span class="sxs-lookup"><span data-stu-id="1130f-129">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.</span></span>|
|<span data-ttu-id="1130f-130">operator</span><span class="sxs-lookup"><span data-stu-id="1130f-130">operator</span></span>|[<span data-ttu-id="1130f-131">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="1130f-131">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="1130f-132">O operador para detecção de arquivo ou pasta.</span><span class="sxs-lookup"><span data-stu-id="1130f-132">The operator for file or folder detection.</span></span> <span data-ttu-id="1130f-133">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="1130f-133">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="1130f-134">ComparisonValue</span><span class="sxs-lookup"><span data-stu-id="1130f-134">comparisonValue</span></span>|<span data-ttu-id="1130f-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1130f-135">String</span></span>|<span data-ttu-id="1130f-136">O valor de comparação de arquivo ou pasta.</span><span class="sxs-lookup"><span data-stu-id="1130f-136">The file or folder comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1130f-137">Relações</span><span class="sxs-lookup"><span data-stu-id="1130f-137">Relationships</span></span>
<span data-ttu-id="1130f-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1130f-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1130f-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1130f-139">JSON Representation</span></span>
<span data-ttu-id="1130f-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1130f-140">Here is a JSON representation of the resource.</span></span>
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





