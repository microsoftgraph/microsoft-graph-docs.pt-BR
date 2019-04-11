---
title: tipo de recurso win32LobAppPowerShellScriptDetection
description: Contém propriedades de script do PowerShell para detectar um aplicativo Win32
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ca55a55ea17dcd032204dcb786ea07a9801f4674
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785640"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="29ae2-103">tipo de recurso win32LobAppPowerShellScriptDetection</span><span class="sxs-lookup"><span data-stu-id="29ae2-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="29ae2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="29ae2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29ae2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="29ae2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29ae2-106">Contém propriedades de script do PowerShell para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="29ae2-106">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="29ae2-107">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="29ae2-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="29ae2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="29ae2-108">Properties</span></span>
|<span data-ttu-id="29ae2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29ae2-109">Property</span></span>|<span data-ttu-id="29ae2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="29ae2-110">Type</span></span>|<span data-ttu-id="29ae2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="29ae2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29ae2-112">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="29ae2-112">enforceSignatureCheck</span></span>|<span data-ttu-id="29ae2-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="29ae2-113">Boolean</span></span>|<span data-ttu-id="29ae2-114">Um valor que indica se a verificação de assinatura é imposta</span><span class="sxs-lookup"><span data-stu-id="29ae2-114">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="29ae2-115">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="29ae2-115">runAs32Bit</span></span>|<span data-ttu-id="29ae2-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="29ae2-116">Boolean</span></span>|<span data-ttu-id="29ae2-117">Um valor que indica se este script deve ser executado como 32 bits</span><span class="sxs-lookup"><span data-stu-id="29ae2-117">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="29ae2-118">scriptContent</span><span class="sxs-lookup"><span data-stu-id="29ae2-118">scriptContent</span></span>|<span data-ttu-id="29ae2-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="29ae2-119">String</span></span>|<span data-ttu-id="29ae2-120">O conteúdo de script codificado em base64 para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="29ae2-120">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="29ae2-121">Relações</span><span class="sxs-lookup"><span data-stu-id="29ae2-121">Relationships</span></span>
<span data-ttu-id="29ae2-122">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="29ae2-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="29ae2-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="29ae2-123">JSON Representation</span></span>
<span data-ttu-id="29ae2-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="29ae2-124">Here is a JSON representation of the resource.</span></span>
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





