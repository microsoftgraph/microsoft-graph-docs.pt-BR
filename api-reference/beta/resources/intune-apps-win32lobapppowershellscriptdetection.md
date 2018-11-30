---
title: tipo de recurso de win32LobAppPowerShellScriptDetection
description: Contém propriedades de script do PowerShell para detectar um aplicativo Win32
ms.openlocfilehash: e5d87d3d2a90c0ac7f8ce6db7e14b105583a76f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036955"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="cf334-103">tipo de recurso de win32LobAppPowerShellScriptDetection</span><span class="sxs-lookup"><span data-stu-id="cf334-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="cf334-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cf334-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf334-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cf334-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cf334-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cf334-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf334-107">Contém propriedades de script do PowerShell para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="cf334-107">Contains PowerShell script properties to detect a Win32 App</span></span>

<span data-ttu-id="cf334-108">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="cf334-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cf334-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf334-109">Properties</span></span>
|<span data-ttu-id="cf334-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf334-110">Property</span></span>|<span data-ttu-id="cf334-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf334-111">Type</span></span>|<span data-ttu-id="cf334-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf334-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf334-113">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="cf334-113">enforceSignatureCheck</span></span>|<span data-ttu-id="cf334-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="cf334-114">Boolean</span></span>|<span data-ttu-id="cf334-115">Um valor que indica se a verificação da assinatura será aplicada.</span><span class="sxs-lookup"><span data-stu-id="cf334-115">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="cf334-116">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="cf334-116">runAs32Bit</span></span>|<span data-ttu-id="cf334-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="cf334-117">Boolean</span></span>|<span data-ttu-id="cf334-118">Um valor que indica se esse script deve ser executado como de 32 bits</span><span class="sxs-lookup"><span data-stu-id="cf334-118">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="cf334-119">scriptContent</span><span class="sxs-lookup"><span data-stu-id="cf334-119">scriptContent</span></span>|<span data-ttu-id="cf334-120">String</span><span class="sxs-lookup"><span data-stu-id="cf334-120">String</span></span>|<span data-ttu-id="cf334-121">O base64 codificado conteúdo de script para detectar app Win32 linha de negócios (LoB)</span><span class="sxs-lookup"><span data-stu-id="cf334-121">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf334-122">Relações</span><span class="sxs-lookup"><span data-stu-id="cf334-122">Relationships</span></span>
<span data-ttu-id="cf334-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cf334-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cf334-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cf334-124">JSON Representation</span></span>
<span data-ttu-id="cf334-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cf334-125">Here is a JSON representation of the resource.</span></span>
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





