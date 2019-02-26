---
title: tipo de recurso win32LobAppPowerShellScriptDetection
description: Contém propriedades de script do PowerShell para detectar um aplicativo Win32
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa5452fd9e73aef846d0b6de86a2b84e2c42ba26
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168520"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="33f4b-103">tipo de recurso win32LobAppPowerShellScriptDetection</span><span class="sxs-lookup"><span data-stu-id="33f4b-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="33f4b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="33f4b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33f4b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="33f4b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33f4b-106">Contém propriedades de script do PowerShell para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="33f4b-106">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="33f4b-107">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="33f4b-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="33f4b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="33f4b-108">Properties</span></span>
|<span data-ttu-id="33f4b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33f4b-109">Property</span></span>|<span data-ttu-id="33f4b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="33f4b-110">Type</span></span>|<span data-ttu-id="33f4b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="33f4b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33f4b-112">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="33f4b-112">enforceSignatureCheck</span></span>|<span data-ttu-id="33f4b-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="33f4b-113">Boolean</span></span>|<span data-ttu-id="33f4b-114">Um valor que indica se a verificação de assinatura é imposta</span><span class="sxs-lookup"><span data-stu-id="33f4b-114">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="33f4b-115">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="33f4b-115">runAs32Bit</span></span>|<span data-ttu-id="33f4b-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="33f4b-116">Boolean</span></span>|<span data-ttu-id="33f4b-117">Um valor que indica se este script deve ser executado como 32 bits</span><span class="sxs-lookup"><span data-stu-id="33f4b-117">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="33f4b-118">scriptContent</span><span class="sxs-lookup"><span data-stu-id="33f4b-118">scriptContent</span></span>|<span data-ttu-id="33f4b-119">String</span><span class="sxs-lookup"><span data-stu-id="33f4b-119">String</span></span>|<span data-ttu-id="33f4b-120">O conteúdo de script codificado em base64 para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="33f4b-120">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="33f4b-121">Relações</span><span class="sxs-lookup"><span data-stu-id="33f4b-121">Relationships</span></span>
<span data-ttu-id="33f4b-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="33f4b-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="33f4b-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="33f4b-123">JSON Representation</span></span>
<span data-ttu-id="33f4b-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="33f4b-124">Here is a JSON representation of the resource.</span></span>
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




