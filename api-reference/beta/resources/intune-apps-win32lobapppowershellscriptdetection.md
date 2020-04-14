---
title: tipo de recurso win32LobAppPowerShellScriptDetection
description: Contém propriedades de script do PowerShell para detectar um aplicativo Win32
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d36591c566e93f9cf4d0c6a7e300224e74033a1b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422916"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="54dac-103">tipo de recurso win32LobAppPowerShellScriptDetection</span><span class="sxs-lookup"><span data-stu-id="54dac-103">win32LobAppPowerShellScriptDetection resource type</span></span>

<span data-ttu-id="54dac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54dac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54dac-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="54dac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54dac-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="54dac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54dac-107">Contém propriedades de script do PowerShell para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="54dac-107">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="54dac-108">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="54dac-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="54dac-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="54dac-109">Properties</span></span>
|<span data-ttu-id="54dac-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="54dac-110">Property</span></span>|<span data-ttu-id="54dac-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="54dac-111">Type</span></span>|<span data-ttu-id="54dac-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="54dac-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54dac-113">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="54dac-113">enforceSignatureCheck</span></span>|<span data-ttu-id="54dac-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="54dac-114">Boolean</span></span>|<span data-ttu-id="54dac-115">Um valor que indica se a verificação de assinatura é imposta</span><span class="sxs-lookup"><span data-stu-id="54dac-115">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="54dac-116">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="54dac-116">runAs32Bit</span></span>|<span data-ttu-id="54dac-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="54dac-117">Boolean</span></span>|<span data-ttu-id="54dac-118">Um valor que indica se este script deve ser executado como 32 bits</span><span class="sxs-lookup"><span data-stu-id="54dac-118">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="54dac-119">scriptContent</span><span class="sxs-lookup"><span data-stu-id="54dac-119">scriptContent</span></span>|<span data-ttu-id="54dac-120">String</span><span class="sxs-lookup"><span data-stu-id="54dac-120">String</span></span>|<span data-ttu-id="54dac-121">O conteúdo de script codificado em base64 para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="54dac-121">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="54dac-122">Relações</span><span class="sxs-lookup"><span data-stu-id="54dac-122">Relationships</span></span>
<span data-ttu-id="54dac-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="54dac-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54dac-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="54dac-124">JSON Representation</span></span>
<span data-ttu-id="54dac-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="54dac-125">Here is a JSON representation of the resource.</span></span>
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



