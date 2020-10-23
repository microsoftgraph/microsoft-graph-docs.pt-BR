---
title: tipo de recurso win32LobAppPowerShellScriptRequirement
description: Contém propriedades de script do PowerShell para detectar um aplicativo Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 262800b2285ba2483f97f35f0d39f9d3e7209ee0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694044"
---
# <a name="win32lobapppowershellscriptrequirement-resource-type"></a><span data-ttu-id="03e88-103">tipo de recurso win32LobAppPowerShellScriptRequirement</span><span class="sxs-lookup"><span data-stu-id="03e88-103">win32LobAppPowerShellScriptRequirement resource type</span></span>

<span data-ttu-id="03e88-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03e88-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03e88-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="03e88-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03e88-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="03e88-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03e88-107">Contém propriedades de script do PowerShell para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="03e88-107">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="03e88-108">Herda de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="03e88-108">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="03e88-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="03e88-109">Properties</span></span>
|<span data-ttu-id="03e88-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="03e88-110">Property</span></span>|<span data-ttu-id="03e88-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="03e88-111">Type</span></span>|<span data-ttu-id="03e88-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="03e88-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03e88-113">operator</span><span class="sxs-lookup"><span data-stu-id="03e88-113">operator</span></span>|[<span data-ttu-id="03e88-114">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="03e88-114">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="03e88-115">O operador para detecção herdada de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span><span class="sxs-lookup"><span data-stu-id="03e88-115">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="03e88-116">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="03e88-116">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="03e88-117">detecçaovalue</span><span class="sxs-lookup"><span data-stu-id="03e88-117">detectionValue</span></span>|<span data-ttu-id="03e88-118">String</span><span class="sxs-lookup"><span data-stu-id="03e88-118">String</span></span>|<span data-ttu-id="03e88-119">O valor de detecção herdado de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="03e88-119">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="03e88-120">displayName</span><span class="sxs-lookup"><span data-stu-id="03e88-120">displayName</span></span>|<span data-ttu-id="03e88-121">String</span><span class="sxs-lookup"><span data-stu-id="03e88-121">String</span></span>|<span data-ttu-id="03e88-122">O nome de exibição exclusivo para esta regra</span><span class="sxs-lookup"><span data-stu-id="03e88-122">The unique display name for this rule</span></span>|
|<span data-ttu-id="03e88-123">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="03e88-123">enforceSignatureCheck</span></span>|<span data-ttu-id="03e88-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="03e88-124">Boolean</span></span>|<span data-ttu-id="03e88-125">Um valor que indica se a verificação de assinatura é imposta</span><span class="sxs-lookup"><span data-stu-id="03e88-125">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="03e88-126">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="03e88-126">runAs32Bit</span></span>|<span data-ttu-id="03e88-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="03e88-127">Boolean</span></span>|<span data-ttu-id="03e88-128">Um valor que indica se este script deve ser executado como 32 bits</span><span class="sxs-lookup"><span data-stu-id="03e88-128">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="03e88-129">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="03e88-129">runAsAccount</span></span>|[<span data-ttu-id="03e88-130">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="03e88-130">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="03e88-131">Indica o tipo de contexto de execução em que o script é executado.</span><span class="sxs-lookup"><span data-stu-id="03e88-131">Indicates the type of execution context the script runs in.</span></span> <span data-ttu-id="03e88-132">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="03e88-132">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="03e88-133">scriptContent</span><span class="sxs-lookup"><span data-stu-id="03e88-133">scriptContent</span></span>|<span data-ttu-id="03e88-134">String</span><span class="sxs-lookup"><span data-stu-id="03e88-134">String</span></span>|<span data-ttu-id="03e88-135">O conteúdo de script codificado em base64 para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="03e88-135">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="03e88-136">Detecção</span><span class="sxs-lookup"><span data-stu-id="03e88-136">detectionType</span></span>|[<span data-ttu-id="03e88-137">win32LobAppPowerShellScriptDetectionType</span><span class="sxs-lookup"><span data-stu-id="03e88-137">win32LobAppPowerShellScriptDetectionType</span></span>](../resources/intune-apps-win32lobapppowershellscriptdetectiontype.md)|<span data-ttu-id="03e88-138">O tipo de detecção para saída de script.</span><span class="sxs-lookup"><span data-stu-id="03e88-138">The detection type for script output.</span></span> <span data-ttu-id="03e88-139">Os valores possíveis são: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span><span class="sxs-lookup"><span data-stu-id="03e88-139">Possible values are: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03e88-140">Relações</span><span class="sxs-lookup"><span data-stu-id="03e88-140">Relationships</span></span>
<span data-ttu-id="03e88-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="03e88-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="03e88-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="03e88-142">JSON Representation</span></span>
<span data-ttu-id="03e88-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="03e88-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptRequirement",
  "operator": "String",
  "detectionValue": "String",
  "displayName": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "runAsAccount": "String",
  "scriptContent": "String",
  "detectionType": "String"
}
```





