---
title: tipo de recurso win32LobAppPowerShellScriptDetection
description: Contém propriedades de script do PowerShell para detectar um aplicativo Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 440f86e0056c45f325a9a9bd88f737a91c8efb2a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949672"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="28364-103">tipo de recurso win32LobAppPowerShellScriptDetection</span><span class="sxs-lookup"><span data-stu-id="28364-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="28364-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="28364-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28364-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="28364-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28364-106">Contém propriedades de script do PowerShell para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="28364-106">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="28364-107">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="28364-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="28364-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="28364-108">Properties</span></span>
|<span data-ttu-id="28364-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28364-109">Property</span></span>|<span data-ttu-id="28364-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="28364-110">Type</span></span>|<span data-ttu-id="28364-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="28364-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28364-112">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="28364-112">enforceSignatureCheck</span></span>|<span data-ttu-id="28364-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="28364-113">Boolean</span></span>|<span data-ttu-id="28364-114">Um valor que indica se a verificação de assinatura é imposta</span><span class="sxs-lookup"><span data-stu-id="28364-114">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="28364-115">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="28364-115">runAs32Bit</span></span>|<span data-ttu-id="28364-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="28364-116">Boolean</span></span>|<span data-ttu-id="28364-117">Um valor que indica se este script deve ser executado como 32 bits</span><span class="sxs-lookup"><span data-stu-id="28364-117">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="28364-118">scriptContent</span><span class="sxs-lookup"><span data-stu-id="28364-118">scriptContent</span></span>|<span data-ttu-id="28364-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="28364-119">String</span></span>|<span data-ttu-id="28364-120">O conteúdo de script codificado em base64 para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="28364-120">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="28364-121">Relações</span><span class="sxs-lookup"><span data-stu-id="28364-121">Relationships</span></span>
<span data-ttu-id="28364-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="28364-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="28364-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="28364-123">JSON Representation</span></span>
<span data-ttu-id="28364-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="28364-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptDetection",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "scriptContent": "String"
}
```




