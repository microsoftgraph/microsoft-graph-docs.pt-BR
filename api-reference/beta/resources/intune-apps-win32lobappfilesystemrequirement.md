---
title: tipo de recurso win32LobAppFileSystemRequirement
description: Contém um caminho de arquivo ou pasta para detectar um aplicativo Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 498e4b953b283ac0a0cffa6a7a21ea91232b724b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949588"
---
# <a name="win32lobappfilesystemrequirement-resource-type"></a><span data-ttu-id="3a79f-103">tipo de recurso win32LobAppFileSystemRequirement</span><span class="sxs-lookup"><span data-stu-id="3a79f-103">win32LobAppFileSystemRequirement resource type</span></span>

> <span data-ttu-id="3a79f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3a79f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a79f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3a79f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a79f-106">Contém um caminho de arquivo ou pasta para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="3a79f-106">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="3a79f-107">Herda de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="3a79f-107">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3a79f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a79f-108">Properties</span></span>
|<span data-ttu-id="3a79f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3a79f-109">Property</span></span>|<span data-ttu-id="3a79f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a79f-110">Type</span></span>|<span data-ttu-id="3a79f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a79f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a79f-112">operator</span><span class="sxs-lookup"><span data-stu-id="3a79f-112">operator</span></span>|[<span data-ttu-id="3a79f-113">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="3a79f-113">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="3a79f-114">O operador para detecção herdada de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span><span class="sxs-lookup"><span data-stu-id="3a79f-114">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="3a79f-115">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="3a79f-115">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="3a79f-116">detecçaovalue</span><span class="sxs-lookup"><span data-stu-id="3a79f-116">detectionValue</span></span>|<span data-ttu-id="3a79f-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a79f-117">String</span></span>|<span data-ttu-id="3a79f-118">O valor de detecção herdado de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="3a79f-118">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="3a79f-119">caminho</span><span class="sxs-lookup"><span data-stu-id="3a79f-119">path</span></span>|<span data-ttu-id="3a79f-120">String</span><span class="sxs-lookup"><span data-stu-id="3a79f-120">String</span></span>|<span data-ttu-id="3a79f-121">O caminho do arquivo ou da pasta para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="3a79f-121">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="3a79f-122">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="3a79f-122">fileOrFolderName</span></span>|<span data-ttu-id="3a79f-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3a79f-123">String</span></span>|<span data-ttu-id="3a79f-124">O nome do arquivo ou pasta para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="3a79f-124">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="3a79f-125">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="3a79f-125">check32BitOn64System</span></span>|<span data-ttu-id="3a79f-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="3a79f-126">Boolean</span></span>|<span data-ttu-id="3a79f-127">Um valor que indica se este arquivo ou pasta é para verificar o aplicativo de 32 bits no sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="3a79f-127">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="3a79f-128">Detecção</span><span class="sxs-lookup"><span data-stu-id="3a79f-128">detectionType</span></span>|[<span data-ttu-id="3a79f-129">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="3a79f-129">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="3a79f-130">O tipo de detecção do sistema de arquivos.</span><span class="sxs-lookup"><span data-stu-id="3a79f-130">The file system detection type.</span></span> <span data-ttu-id="3a79f-131">Os valores possíveis são: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span><span class="sxs-lookup"><span data-stu-id="3a79f-131">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a79f-132">Relações</span><span class="sxs-lookup"><span data-stu-id="3a79f-132">Relationships</span></span>
<span data-ttu-id="3a79f-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3a79f-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a79f-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a79f-134">JSON Representation</span></span>
<span data-ttu-id="3a79f-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a79f-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemRequirement",
  "operator": "String",
  "detectionValue": "String",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": true,
  "detectionType": "String"
}
```




