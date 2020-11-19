---
title: tipo de recurso win32LobAppPowerShellScriptDetection
description: Contém propriedades de script do PowerShell para detectar um aplicativo Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 507b7adfe3a6d69df99063e69c3651848fc70e22
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273960"
---
# <a name="win32lobapppowershellscriptdetection-resource-type"></a><span data-ttu-id="7bed9-103">tipo de recurso win32LobAppPowerShellScriptDetection</span><span class="sxs-lookup"><span data-stu-id="7bed9-103">win32LobAppPowerShellScriptDetection resource type</span></span>

<span data-ttu-id="7bed9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bed9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7bed9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7bed9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7bed9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7bed9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bed9-107">Contém propriedades de script do PowerShell para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="7bed9-107">Contains PowerShell script properties to detect a Win32 App</span></span>


<span data-ttu-id="7bed9-108">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="7bed9-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7bed9-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7bed9-109">Properties</span></span>
|<span data-ttu-id="7bed9-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7bed9-110">Property</span></span>|<span data-ttu-id="7bed9-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bed9-111">Type</span></span>|<span data-ttu-id="7bed9-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bed9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bed9-113">enforceSignatureCheck</span><span class="sxs-lookup"><span data-stu-id="7bed9-113">enforceSignatureCheck</span></span>|<span data-ttu-id="7bed9-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="7bed9-114">Boolean</span></span>|<span data-ttu-id="7bed9-115">Um valor que indica se a verificação de assinatura é imposta</span><span class="sxs-lookup"><span data-stu-id="7bed9-115">A value indicating whether signature check is enforced</span></span>|
|<span data-ttu-id="7bed9-116">runAs32Bit</span><span class="sxs-lookup"><span data-stu-id="7bed9-116">runAs32Bit</span></span>|<span data-ttu-id="7bed9-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="7bed9-117">Boolean</span></span>|<span data-ttu-id="7bed9-118">Um valor que indica se este script deve ser executado como 32 bits</span><span class="sxs-lookup"><span data-stu-id="7bed9-118">A value indicating whether this script should run as 32-bit</span></span>|
|<span data-ttu-id="7bed9-119">scriptContent</span><span class="sxs-lookup"><span data-stu-id="7bed9-119">scriptContent</span></span>|<span data-ttu-id="7bed9-120">String</span><span class="sxs-lookup"><span data-stu-id="7bed9-120">String</span></span>|<span data-ttu-id="7bed9-121">O conteúdo de script codificado em base64 para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="7bed9-121">The base64 encoded script content to detect Win32 Line of Business (LoB) app</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bed9-122">Relações</span><span class="sxs-lookup"><span data-stu-id="7bed9-122">Relationships</span></span>
<span data-ttu-id="7bed9-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7bed9-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7bed9-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7bed9-124">JSON Representation</span></span>
<span data-ttu-id="7bed9-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7bed9-125">Here is a JSON representation of the resource.</span></span>
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




