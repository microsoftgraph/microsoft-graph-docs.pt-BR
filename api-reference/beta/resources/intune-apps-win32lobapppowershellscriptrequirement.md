---
title: tipo de recurso win32LobAppPowerShellScriptRequirement
description: Contém propriedades de script do PowerShell para detectar um aplicativo Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a85a777f0dd888296250627b6bab05d0c87dc14c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987338"
---
# <a name="win32lobapppowershellscriptrequirement-resource-type"></a><span data-ttu-id="6825d-103">tipo de recurso win32LobAppPowerShellScriptRequirement</span><span class="sxs-lookup"><span data-stu-id="6825d-103">win32LobAppPowerShellScriptRequirement resource type</span></span>

> <span data-ttu-id="6825d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6825d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6825d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6825d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6825d-106">Contém propriedades de script do PowerShell para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="6825d-106">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="6825d-107">Herda de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="6825d-107">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6825d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6825d-108">Properties</span></span>
|<span data-ttu-id="6825d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6825d-109">Property</span></span>|<span data-ttu-id="6825d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6825d-110">Type</span></span>|<span data-ttu-id="6825d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6825d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6825d-112">operator</span><span class="sxs-lookup"><span data-stu-id="6825d-112">operator</span></span>|[<span data-ttu-id="6825d-113">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="6825d-113">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="6825d-114">O operador para detecção herdada de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span><span class="sxs-lookup"><span data-stu-id="6825d-114">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="6825d-115">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="6825d-115">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="6825d-116">detecçaovalue</span><span class="sxs-lookup"><span data-stu-id="6825d-116">detectionValue</span></span>|<span data-ttu-id="6825d-117">String</span><span class="sxs-lookup"><span data-stu-id="6825d-117">String</span></span>|<span data-ttu-id="6825d-118">O valor de detecção herdado de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="6825d-118">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="6825d-119">displayName</span><span class="sxs-lookup"><span data-stu-id="6825d-119">displayName</span></span>|<span data-ttu-id="6825d-120">String</span><span class="sxs-lookup"><span data-stu-id="6825d-120">String</span></span>|<span data-ttu-id="6825d-121">O nome de exibição exclusivo para esta regra</span><span class="sxs-lookup"><span data-stu-id="6825d-121">The unique display name for this rule</span></span>|
|<span data-ttu-id="6825d-122">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="6825d-122">enforceSignatureCheck</span></span>|<span data-ttu-id="6825d-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="6825d-123">Boolean</span></span>|<span data-ttu-id="6825d-124">Um valor que indica se a verificação de assinatura é imposta</span><span class="sxs-lookup"><span data-stu-id="6825d-124">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="6825d-125">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="6825d-125">runAs32Bit</span></span>|<span data-ttu-id="6825d-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="6825d-126">Boolean</span></span>|<span data-ttu-id="6825d-127">Um valor que indica se este script deve ser executado como 32 bits</span><span class="sxs-lookup"><span data-stu-id="6825d-127">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="6825d-128">runAsAccount</span><span class="sxs-lookup"><span data-stu-id="6825d-128">runAsAccount</span></span>|[<span data-ttu-id="6825d-129">runAsAccountType</span><span class="sxs-lookup"><span data-stu-id="6825d-129">runAsAccountType</span></span>](../resources/intune-shared-runasaccounttype.md)|<span data-ttu-id="6825d-130">Indica o tipo de contexto de execução em que o script é executado.</span><span class="sxs-lookup"><span data-stu-id="6825d-130">Indicates the type of execution context the script runs in.</span></span> <span data-ttu-id="6825d-131">Os valores possíveis são: `system` e `user`.</span><span class="sxs-lookup"><span data-stu-id="6825d-131">Possible values are: `system`, `user`.</span></span>|
|<span data-ttu-id="6825d-132">scriptContent</span><span class="sxs-lookup"><span data-stu-id="6825d-132">scriptContent</span></span>|<span data-ttu-id="6825d-133">String</span><span class="sxs-lookup"><span data-stu-id="6825d-133">String</span></span>|<span data-ttu-id="6825d-134">O conteúdo de script codificado em base64 para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="6825d-134">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="6825d-135">Detecção</span><span class="sxs-lookup"><span data-stu-id="6825d-135">detectionType</span></span>|[<span data-ttu-id="6825d-136">win32LobAppPowerShellScriptDetectionType</span><span class="sxs-lookup"><span data-stu-id="6825d-136">win32LobAppPowerShellScriptDetectionType</span></span>](../resources/intune-apps-win32lobapppowershellscriptdetectiontype.md)|<span data-ttu-id="6825d-137">O tipo de detecção para saída de script.</span><span class="sxs-lookup"><span data-stu-id="6825d-137">The detection type for script output.</span></span> <span data-ttu-id="6825d-138">Os valores possíveis são: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span><span class="sxs-lookup"><span data-stu-id="6825d-138">Possible values are: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6825d-139">Relações</span><span class="sxs-lookup"><span data-stu-id="6825d-139">Relationships</span></span>
<span data-ttu-id="6825d-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6825d-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6825d-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6825d-141">JSON Representation</span></span>
<span data-ttu-id="6825d-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6825d-142">Here is a JSON representation of the resource.</span></span>
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





