---
title: Tipo de recurso win32LobAppFileSystemRule
description: Um tipo complexo para armazenar dados de regra de arquivo ou pasta para um aplicativo LOB win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a0c8a45a9f3d49c671949a2b5ad3b9bd549ee8d7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752396"
---
# <a name="win32lobappfilesystemrule-resource-type"></a><span data-ttu-id="d93d1-103">Tipo de recurso win32LobAppFileSystemRule</span><span class="sxs-lookup"><span data-stu-id="d93d1-103">win32LobAppFileSystemRule resource type</span></span>

<span data-ttu-id="d93d1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d93d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d93d1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d93d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d93d1-106">Um tipo complexo para armazenar dados de regra de arquivo ou pasta para um aplicativo LOB win32.</span><span class="sxs-lookup"><span data-stu-id="d93d1-106">A complex type to store file or folder rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="d93d1-107">Herda de [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="d93d1-107">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d93d1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d93d1-108">Properties</span></span>
|<span data-ttu-id="d93d1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d93d1-109">Property</span></span>|<span data-ttu-id="d93d1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d93d1-110">Type</span></span>|<span data-ttu-id="d93d1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d93d1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d93d1-112">ruleType</span><span class="sxs-lookup"><span data-stu-id="d93d1-112">ruleType</span></span>|[<span data-ttu-id="d93d1-113">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="d93d1-113">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="d93d1-114">O tipo de regra que indica a finalidade da regra.</span><span class="sxs-lookup"><span data-stu-id="d93d1-114">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="d93d1-115">Herdado [de win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="d93d1-115">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="d93d1-116">Os valores possíveis são: `detection` e `requirement`.</span><span class="sxs-lookup"><span data-stu-id="d93d1-116">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="d93d1-117">caminho</span><span class="sxs-lookup"><span data-stu-id="d93d1-117">path</span></span>|<span data-ttu-id="d93d1-118">String</span><span class="sxs-lookup"><span data-stu-id="d93d1-118">String</span></span>|<span data-ttu-id="d93d1-119">O arquivo ou o caminho da pasta a ser olhado para cima.</span><span class="sxs-lookup"><span data-stu-id="d93d1-119">The file or folder path to look up.</span></span>|
|<span data-ttu-id="d93d1-120">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="d93d1-120">fileOrFolderName</span></span>|<span data-ttu-id="d93d1-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d93d1-121">String</span></span>|<span data-ttu-id="d93d1-122">O arquivo ou o nome da pasta a ser olhado.</span><span class="sxs-lookup"><span data-stu-id="d93d1-122">The file or folder name to look up.</span></span>|
|<span data-ttu-id="d93d1-123">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="d93d1-123">check32BitOn64System</span></span>|<span data-ttu-id="d93d1-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="d93d1-124">Boolean</span></span>|<span data-ttu-id="d93d1-125">Um valor que indica se as variáveis de ambiente devem ser expandidas no contexto de 32 bits em sistemas de 64 bits.</span><span class="sxs-lookup"><span data-stu-id="d93d1-125">A value indicating whether to expand environment variables in the 32-bit context on 64-bit systems.</span></span>|
|<span data-ttu-id="d93d1-126">operationType</span><span class="sxs-lookup"><span data-stu-id="d93d1-126">operationType</span></span>|[<span data-ttu-id="d93d1-127">win32LobAppFileSystemOperationType</span><span class="sxs-lookup"><span data-stu-id="d93d1-127">win32LobAppFileSystemOperationType</span></span>](../resources/intune-apps-win32lobappfilesystemoperationtype.md)|<span data-ttu-id="d93d1-128">O tipo de operação do sistema de arquivos.</span><span class="sxs-lookup"><span data-stu-id="d93d1-128">The file system operation type.</span></span> <span data-ttu-id="d93d1-129">Os possíveis valores são: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.</span><span class="sxs-lookup"><span data-stu-id="d93d1-129">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.</span></span>|
|<span data-ttu-id="d93d1-130">operator</span><span class="sxs-lookup"><span data-stu-id="d93d1-130">operator</span></span>|[<span data-ttu-id="d93d1-131">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="d93d1-131">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="d93d1-132">O operador para detecção de arquivo ou pasta.</span><span class="sxs-lookup"><span data-stu-id="d93d1-132">The operator for file or folder detection.</span></span> <span data-ttu-id="d93d1-133">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="d93d1-133">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="d93d1-134">comparisonValue</span><span class="sxs-lookup"><span data-stu-id="d93d1-134">comparisonValue</span></span>|<span data-ttu-id="d93d1-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d93d1-135">String</span></span>|<span data-ttu-id="d93d1-136">O valor de comparação de arquivo ou pasta.</span><span class="sxs-lookup"><span data-stu-id="d93d1-136">The file or folder comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d93d1-137">Relações</span><span class="sxs-lookup"><span data-stu-id="d93d1-137">Relationships</span></span>
<span data-ttu-id="d93d1-138">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d93d1-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d93d1-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d93d1-139">JSON Representation</span></span>
<span data-ttu-id="d93d1-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d93d1-140">Here is a JSON representation of the resource.</span></span>
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




