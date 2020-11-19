---
title: tipo de recurso win32LobAppFileSystemDetection
description: Contém um caminho de arquivo ou pasta para detectar um aplicativo Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3c3d4d3ef791b4e0056ae0410c1e576a313af0f3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49217090"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a><span data-ttu-id="160b8-103">tipo de recurso win32LobAppFileSystemDetection</span><span class="sxs-lookup"><span data-stu-id="160b8-103">win32LobAppFileSystemDetection resource type</span></span>

<span data-ttu-id="160b8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="160b8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="160b8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="160b8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="160b8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="160b8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="160b8-107">Contém um caminho de arquivo ou pasta para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="160b8-107">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="160b8-108">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="160b8-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="160b8-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="160b8-109">Properties</span></span>
|<span data-ttu-id="160b8-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="160b8-110">Property</span></span>|<span data-ttu-id="160b8-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="160b8-111">Type</span></span>|<span data-ttu-id="160b8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="160b8-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="160b8-113">caminho</span><span class="sxs-lookup"><span data-stu-id="160b8-113">path</span></span>|<span data-ttu-id="160b8-114">String</span><span class="sxs-lookup"><span data-stu-id="160b8-114">String</span></span>|<span data-ttu-id="160b8-115">O caminho do arquivo ou da pasta para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="160b8-115">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="160b8-116">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="160b8-116">fileOrFolderName</span></span>|<span data-ttu-id="160b8-117">String</span><span class="sxs-lookup"><span data-stu-id="160b8-117">String</span></span>|<span data-ttu-id="160b8-118">O nome do arquivo ou pasta para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="160b8-118">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="160b8-119">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="160b8-119">check32BitOn64System</span></span>|<span data-ttu-id="160b8-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="160b8-120">Boolean</span></span>|<span data-ttu-id="160b8-121">Um valor que indica se este arquivo ou pasta é para verificar o aplicativo de 32 bits no sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="160b8-121">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="160b8-122">Detecção</span><span class="sxs-lookup"><span data-stu-id="160b8-122">detectionType</span></span>|[<span data-ttu-id="160b8-123">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="160b8-123">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="160b8-124">O tipo de detecção do sistema de arquivos.</span><span class="sxs-lookup"><span data-stu-id="160b8-124">The file system detection type.</span></span> <span data-ttu-id="160b8-125">Os valores possíveis são: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span><span class="sxs-lookup"><span data-stu-id="160b8-125">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|
|<span data-ttu-id="160b8-126">operator</span><span class="sxs-lookup"><span data-stu-id="160b8-126">operator</span></span>|[<span data-ttu-id="160b8-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="160b8-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="160b8-128">O operador para detecção de arquivo ou pasta.</span><span class="sxs-lookup"><span data-stu-id="160b8-128">The operator for file or folder detection.</span></span> <span data-ttu-id="160b8-129">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="160b8-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="160b8-130">detecçaovalue</span><span class="sxs-lookup"><span data-stu-id="160b8-130">detectionValue</span></span>|<span data-ttu-id="160b8-131">String</span><span class="sxs-lookup"><span data-stu-id="160b8-131">String</span></span>|<span data-ttu-id="160b8-132">O valor de detecção de arquivo ou pasta</span><span class="sxs-lookup"><span data-stu-id="160b8-132">The file or folder detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="160b8-133">Relações</span><span class="sxs-lookup"><span data-stu-id="160b8-133">Relationships</span></span>
<span data-ttu-id="160b8-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="160b8-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="160b8-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="160b8-135">JSON Representation</span></span>
<span data-ttu-id="160b8-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="160b8-136">Here is a JSON representation of the resource.</span></span>
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




