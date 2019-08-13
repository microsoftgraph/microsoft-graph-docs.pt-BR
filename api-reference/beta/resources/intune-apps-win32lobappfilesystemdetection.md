---
title: tipo de recurso win32LobAppFileSystemDetection
description: Contém um caminho de arquivo ou pasta para detectar um aplicativo Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bd18cf615b33faa58e699bd53d93ed2110144c4a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335729"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a><span data-ttu-id="e8c75-103">tipo de recurso win32LobAppFileSystemDetection</span><span class="sxs-lookup"><span data-stu-id="e8c75-103">win32LobAppFileSystemDetection resource type</span></span>

> <span data-ttu-id="e8c75-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e8c75-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8c75-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e8c75-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8c75-106">Contém um caminho de arquivo ou pasta para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="e8c75-106">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="e8c75-107">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="e8c75-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e8c75-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e8c75-108">Properties</span></span>
|<span data-ttu-id="e8c75-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8c75-109">Property</span></span>|<span data-ttu-id="e8c75-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8c75-110">Type</span></span>|<span data-ttu-id="e8c75-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8c75-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8c75-112">caminho</span><span class="sxs-lookup"><span data-stu-id="e8c75-112">path</span></span>|<span data-ttu-id="e8c75-113">String</span><span class="sxs-lookup"><span data-stu-id="e8c75-113">String</span></span>|<span data-ttu-id="e8c75-114">O caminho do arquivo ou da pasta para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="e8c75-114">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="e8c75-115">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="e8c75-115">fileOrFolderName</span></span>|<span data-ttu-id="e8c75-116">String</span><span class="sxs-lookup"><span data-stu-id="e8c75-116">String</span></span>|<span data-ttu-id="e8c75-117">O nome do arquivo ou pasta para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="e8c75-117">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="e8c75-118">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="e8c75-118">check32BitOn64System</span></span>|<span data-ttu-id="e8c75-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="e8c75-119">Boolean</span></span>|<span data-ttu-id="e8c75-120">Um valor que indica se este arquivo ou pasta é para verificar o aplicativo de 32 bits no sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="e8c75-120">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="e8c75-121">Detecção</span><span class="sxs-lookup"><span data-stu-id="e8c75-121">detectionType</span></span>|[<span data-ttu-id="e8c75-122">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="e8c75-122">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="e8c75-123">O tipo de detecção do sistema de arquivos.</span><span class="sxs-lookup"><span data-stu-id="e8c75-123">The file system detection type.</span></span> <span data-ttu-id="e8c75-124">Os valores possíveis são: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span><span class="sxs-lookup"><span data-stu-id="e8c75-124">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|
|<span data-ttu-id="e8c75-125">operator</span><span class="sxs-lookup"><span data-stu-id="e8c75-125">operator</span></span>|[<span data-ttu-id="e8c75-126">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="e8c75-126">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="e8c75-127">O operador para detecção de arquivo ou pasta.</span><span class="sxs-lookup"><span data-stu-id="e8c75-127">The operator for file or folder detection.</span></span> <span data-ttu-id="e8c75-128">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="e8c75-128">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="e8c75-129">detecçaovalue</span><span class="sxs-lookup"><span data-stu-id="e8c75-129">detectionValue</span></span>|<span data-ttu-id="e8c75-130">String</span><span class="sxs-lookup"><span data-stu-id="e8c75-130">String</span></span>|<span data-ttu-id="e8c75-131">O valor de detecção de arquivo ou pasta</span><span class="sxs-lookup"><span data-stu-id="e8c75-131">The file or folder detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8c75-132">Relações</span><span class="sxs-lookup"><span data-stu-id="e8c75-132">Relationships</span></span>
<span data-ttu-id="e8c75-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e8c75-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8c75-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e8c75-134">JSON Representation</span></span>
<span data-ttu-id="e8c75-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e8c75-135">Here is a JSON representation of the resource.</span></span>
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



