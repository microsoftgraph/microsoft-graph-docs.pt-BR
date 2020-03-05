---
title: tipo de recurso win32LobAppPowerShellScriptDetection
description: Contém propriedades de script do PowerShell para detectar um aplicativo Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 024ef2708dae3a6c4b030b41d86abbd4c21b6d49
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42490585"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="57b4e-103">tipo de recurso win32LobAppPowerShellScriptDetection</span><span class="sxs-lookup"><span data-stu-id="57b4e-103">win32LobAppPowerShellScriptDetection resource type</span></span>

<span data-ttu-id="57b4e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="57b4e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57b4e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="57b4e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57b4e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="57b4e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57b4e-107">Contém propriedades de script do PowerShell para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="57b4e-107">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="57b4e-108">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="57b4e-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="57b4e-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="57b4e-109">Properties</span></span>
|<span data-ttu-id="57b4e-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57b4e-110">Property</span></span>|<span data-ttu-id="57b4e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="57b4e-111">Type</span></span>|<span data-ttu-id="57b4e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="57b4e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57b4e-113">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="57b4e-113">enforceSignatureCheck</span></span>|<span data-ttu-id="57b4e-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="57b4e-114">Boolean</span></span>|<span data-ttu-id="57b4e-115">Um valor que indica se a verificação de assinatura é imposta</span><span class="sxs-lookup"><span data-stu-id="57b4e-115">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="57b4e-116">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="57b4e-116">runAs32Bit</span></span>|<span data-ttu-id="57b4e-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="57b4e-117">Boolean</span></span>|<span data-ttu-id="57b4e-118">Um valor que indica se este script deve ser executado como 32 bits</span><span class="sxs-lookup"><span data-stu-id="57b4e-118">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="57b4e-119">scriptContent</span><span class="sxs-lookup"><span data-stu-id="57b4e-119">scriptContent</span></span>|<span data-ttu-id="57b4e-120">String</span><span class="sxs-lookup"><span data-stu-id="57b4e-120">String</span></span>|<span data-ttu-id="57b4e-121">O conteúdo de script codificado em base64 para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="57b4e-121">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="57b4e-122">Relações</span><span class="sxs-lookup"><span data-stu-id="57b4e-122">Relationships</span></span>
<span data-ttu-id="57b4e-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="57b4e-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57b4e-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="57b4e-124">JSON Representation</span></span>
<span data-ttu-id="57b4e-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="57b4e-125">Here is a JSON representation of the resource.</span></span>
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



