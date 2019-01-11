---
title: tipo de recurso de win32LobAppPowerShellScriptDetection
description: Contém propriedades de script do PowerShell para detectar um aplicativo Win32
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bdd3c0e6864a3568b4f1efb7c1c18a25f3e7c84d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863025"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="e75a8-103">tipo de recurso de win32LobAppPowerShellScriptDetection</span><span class="sxs-lookup"><span data-stu-id="e75a8-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="e75a8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e75a8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e75a8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e75a8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e75a8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e75a8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e75a8-107">Contém propriedades de script do PowerShell para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="e75a8-107">Contains PowerShell script properties to detect a Win32 App</span></span>

<span data-ttu-id="e75a8-108">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="e75a8-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e75a8-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e75a8-109">Properties</span></span>
|<span data-ttu-id="e75a8-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e75a8-110">Property</span></span>|<span data-ttu-id="e75a8-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="e75a8-111">Type</span></span>|<span data-ttu-id="e75a8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="e75a8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e75a8-113">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="e75a8-113">enforceSignatureCheck</span></span>|<span data-ttu-id="e75a8-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="e75a8-114">Boolean</span></span>|<span data-ttu-id="e75a8-115">Um valor que indica se a verificação da assinatura será aplicada.</span><span class="sxs-lookup"><span data-stu-id="e75a8-115">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="e75a8-116">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="e75a8-116">runAs32Bit</span></span>|<span data-ttu-id="e75a8-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="e75a8-117">Boolean</span></span>|<span data-ttu-id="e75a8-118">Um valor que indica se esse script deve ser executado como de 32 bits</span><span class="sxs-lookup"><span data-stu-id="e75a8-118">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="e75a8-119">scriptContent</span><span class="sxs-lookup"><span data-stu-id="e75a8-119">scriptContent</span></span>|<span data-ttu-id="e75a8-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e75a8-120">String</span></span>|<span data-ttu-id="e75a8-121">O base64 codificado conteúdo de script para detectar app Win32 linha de negócios (LoB)</span><span class="sxs-lookup"><span data-stu-id="e75a8-121">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="e75a8-122">Relações</span><span class="sxs-lookup"><span data-stu-id="e75a8-122">Relationships</span></span>
<span data-ttu-id="e75a8-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e75a8-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e75a8-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e75a8-124">JSON Representation</span></span>
<span data-ttu-id="e75a8-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e75a8-125">Here is a JSON representation of the resource.</span></span>
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





