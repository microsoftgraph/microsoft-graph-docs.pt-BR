---
title: tipo de recurso win32LobAppFileSystemDetection
description: Contém um caminho de arquivo ou pasta para detectar um aplicativo Win32
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: da95d263af1bf2e217ab5468659b17eed2cb3f8c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797651"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a><span data-ttu-id="1ed46-103">tipo de recurso win32LobAppFileSystemDetection</span><span class="sxs-lookup"><span data-stu-id="1ed46-103">win32LobAppFileSystemDetection resource type</span></span>

> <span data-ttu-id="1ed46-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1ed46-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ed46-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1ed46-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ed46-106">Contém um caminho de arquivo ou pasta para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="1ed46-106">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="1ed46-107">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="1ed46-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1ed46-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ed46-108">Properties</span></span>
|<span data-ttu-id="1ed46-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ed46-109">Property</span></span>|<span data-ttu-id="1ed46-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ed46-110">Type</span></span>|<span data-ttu-id="1ed46-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ed46-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ed46-112">caminho</span><span class="sxs-lookup"><span data-stu-id="1ed46-112">path</span></span>|<span data-ttu-id="1ed46-113">String</span><span class="sxs-lookup"><span data-stu-id="1ed46-113">String</span></span>|<span data-ttu-id="1ed46-114">O caminho do arquivo ou da pasta para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="1ed46-114">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="1ed46-115">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="1ed46-115">fileOrFolderName</span></span>|<span data-ttu-id="1ed46-116">String</span><span class="sxs-lookup"><span data-stu-id="1ed46-116">String</span></span>|<span data-ttu-id="1ed46-117">O nome do arquivo ou pasta para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="1ed46-117">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="1ed46-118">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="1ed46-118">check32BitOn64System</span></span>|<span data-ttu-id="1ed46-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ed46-119">Boolean</span></span>|<span data-ttu-id="1ed46-120">Um valor que indica se este arquivo ou pasta é para verificar o aplicativo de 32 bits no sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="1ed46-120">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="1ed46-121">Detecção</span><span class="sxs-lookup"><span data-stu-id="1ed46-121">detectionType</span></span>|[<span data-ttu-id="1ed46-122">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="1ed46-122">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="1ed46-123">O tipo de detecção do sistema de arquivos.</span><span class="sxs-lookup"><span data-stu-id="1ed46-123">The file system detection type.</span></span> <span data-ttu-id="1ed46-124">Os valores possíveis são: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span><span class="sxs-lookup"><span data-stu-id="1ed46-124">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|
|<span data-ttu-id="1ed46-125">operator</span><span class="sxs-lookup"><span data-stu-id="1ed46-125">operator</span></span>|[<span data-ttu-id="1ed46-126">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="1ed46-126">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="1ed46-127">O operador para detecção de arquivo ou pasta.</span><span class="sxs-lookup"><span data-stu-id="1ed46-127">The operator for file or folder detection.</span></span> <span data-ttu-id="1ed46-128">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="1ed46-128">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="1ed46-129">detecçaovalue</span><span class="sxs-lookup"><span data-stu-id="1ed46-129">detectionValue</span></span>|<span data-ttu-id="1ed46-130">String</span><span class="sxs-lookup"><span data-stu-id="1ed46-130">String</span></span>|<span data-ttu-id="1ed46-131">O valor de detecção de arquivo ou pasta</span><span class="sxs-lookup"><span data-stu-id="1ed46-131">The file or folder detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ed46-132">Relações</span><span class="sxs-lookup"><span data-stu-id="1ed46-132">Relationships</span></span>
<span data-ttu-id="1ed46-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1ed46-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ed46-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ed46-134">JSON Representation</span></span>
<span data-ttu-id="1ed46-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1ed46-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemDetection",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": true,
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```



