---
title: tipo de recurso win32LobAppFileSystemDetection
description: Contém um caminho de arquivo ou pasta para detectar um aplicativo Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e9d7142fe8bc2db33472c9fd2997e069a02ace93
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42490865"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a><span data-ttu-id="57640-103">tipo de recurso win32LobAppFileSystemDetection</span><span class="sxs-lookup"><span data-stu-id="57640-103">win32LobAppFileSystemDetection resource type</span></span>

<span data-ttu-id="57640-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="57640-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57640-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="57640-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57640-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="57640-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57640-107">Contém um caminho de arquivo ou pasta para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="57640-107">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="57640-108">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="57640-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="57640-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="57640-109">Properties</span></span>
|<span data-ttu-id="57640-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57640-110">Property</span></span>|<span data-ttu-id="57640-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="57640-111">Type</span></span>|<span data-ttu-id="57640-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="57640-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57640-113">caminho</span><span class="sxs-lookup"><span data-stu-id="57640-113">path</span></span>|<span data-ttu-id="57640-114">String</span><span class="sxs-lookup"><span data-stu-id="57640-114">String</span></span>|<span data-ttu-id="57640-115">O caminho do arquivo ou da pasta para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="57640-115">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="57640-116">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="57640-116">fileOrFolderName</span></span>|<span data-ttu-id="57640-117">String</span><span class="sxs-lookup"><span data-stu-id="57640-117">String</span></span>|<span data-ttu-id="57640-118">O nome do arquivo ou pasta para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="57640-118">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="57640-119">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="57640-119">check32BitOn64System</span></span>|<span data-ttu-id="57640-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="57640-120">Boolean</span></span>|<span data-ttu-id="57640-121">Um valor que indica se este arquivo ou pasta é para verificar o aplicativo de 32 bits no sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="57640-121">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="57640-122">Detecção</span><span class="sxs-lookup"><span data-stu-id="57640-122">detectionType</span></span>|[<span data-ttu-id="57640-123">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="57640-123">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="57640-124">O tipo de detecção do sistema de arquivos.</span><span class="sxs-lookup"><span data-stu-id="57640-124">The file system detection type.</span></span> <span data-ttu-id="57640-125">Os valores possíveis são: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span><span class="sxs-lookup"><span data-stu-id="57640-125">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|
|<span data-ttu-id="57640-126">operator</span><span class="sxs-lookup"><span data-stu-id="57640-126">operator</span></span>|[<span data-ttu-id="57640-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="57640-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="57640-128">O operador para detecção de arquivo ou pasta.</span><span class="sxs-lookup"><span data-stu-id="57640-128">The operator for file or folder detection.</span></span> <span data-ttu-id="57640-129">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="57640-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="57640-130">detecçaovalue</span><span class="sxs-lookup"><span data-stu-id="57640-130">detectionValue</span></span>|<span data-ttu-id="57640-131">String</span><span class="sxs-lookup"><span data-stu-id="57640-131">String</span></span>|<span data-ttu-id="57640-132">O valor de detecção de arquivo ou pasta</span><span class="sxs-lookup"><span data-stu-id="57640-132">The file or folder detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="57640-133">Relações</span><span class="sxs-lookup"><span data-stu-id="57640-133">Relationships</span></span>
<span data-ttu-id="57640-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="57640-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57640-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="57640-135">JSON Representation</span></span>
<span data-ttu-id="57640-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="57640-136">Here is a JSON representation of the resource.</span></span>
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



