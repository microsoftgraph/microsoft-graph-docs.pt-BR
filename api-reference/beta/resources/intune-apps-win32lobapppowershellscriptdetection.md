---
title: tipo de recurso de win32LobAppPowerShellScriptDetection
description: Contém propriedades de script do PowerShell para detectar um aplicativo Win32
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c5c02228589042d0abf36c34c5818c5a4610514e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399637"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="b8115-103">tipo de recurso de win32LobAppPowerShellScriptDetection</span><span class="sxs-lookup"><span data-stu-id="b8115-103">win32LobAppPowerShellScriptDetection resource type</span></span>

> <span data-ttu-id="b8115-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="b8115-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b8115-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b8115-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b8115-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="b8115-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8115-107">Contém propriedades de script do PowerShell para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="b8115-107">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="b8115-108">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="b8115-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b8115-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b8115-109">Properties</span></span>
|<span data-ttu-id="b8115-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8115-110">Property</span></span>|<span data-ttu-id="b8115-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8115-111">Type</span></span>|<span data-ttu-id="b8115-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8115-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8115-113">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="b8115-113">enforceSignatureCheck</span></span>|<span data-ttu-id="b8115-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8115-114">Boolean</span></span>|<span data-ttu-id="b8115-115">Um valor que indica se a verificação da assinatura será aplicada.</span><span class="sxs-lookup"><span data-stu-id="b8115-115">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="b8115-116">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="b8115-116">runAs32Bit</span></span>|<span data-ttu-id="b8115-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8115-117">Boolean</span></span>|<span data-ttu-id="b8115-118">Um valor que indica se esse script deve ser executado como de 32 bits</span><span class="sxs-lookup"><span data-stu-id="b8115-118">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="b8115-119">scriptContent</span><span class="sxs-lookup"><span data-stu-id="b8115-119">scriptContent</span></span>|<span data-ttu-id="b8115-120">String</span><span class="sxs-lookup"><span data-stu-id="b8115-120">String</span></span>|<span data-ttu-id="b8115-121">O base64 codificado conteúdo de script para detectar app Win32 linha de negócios (LoB)</span><span class="sxs-lookup"><span data-stu-id="b8115-121">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8115-122">Relações</span><span class="sxs-lookup"><span data-stu-id="b8115-122">Relationships</span></span>
<span data-ttu-id="b8115-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b8115-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8115-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b8115-124">JSON Representation</span></span>
<span data-ttu-id="b8115-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b8115-125">Here is a JSON representation of the resource.</span></span>
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




