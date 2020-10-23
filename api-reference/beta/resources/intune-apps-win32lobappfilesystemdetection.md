---
title: tipo de recurso win32LobAppFileSystemDetection
description: Contém um caminho de arquivo ou pasta para detectar um aplicativo Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 55b37904d4195e429b79100300c732772ff42be5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696423"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a><span data-ttu-id="aa0d2-103">tipo de recurso win32LobAppFileSystemDetection</span><span class="sxs-lookup"><span data-stu-id="aa0d2-103">win32LobAppFileSystemDetection resource type</span></span>

<span data-ttu-id="aa0d2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa0d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa0d2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aa0d2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa0d2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aa0d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa0d2-107">Contém um caminho de arquivo ou pasta para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="aa0d2-107">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="aa0d2-108">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="aa0d2-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aa0d2-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aa0d2-109">Properties</span></span>
|<span data-ttu-id="aa0d2-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aa0d2-110">Property</span></span>|<span data-ttu-id="aa0d2-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa0d2-111">Type</span></span>|<span data-ttu-id="aa0d2-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa0d2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa0d2-113">caminho</span><span class="sxs-lookup"><span data-stu-id="aa0d2-113">path</span></span>|<span data-ttu-id="aa0d2-114">String</span><span class="sxs-lookup"><span data-stu-id="aa0d2-114">String</span></span>|<span data-ttu-id="aa0d2-115">O caminho do arquivo ou da pasta para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="aa0d2-115">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="aa0d2-116">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="aa0d2-116">fileOrFolderName</span></span>|<span data-ttu-id="aa0d2-117">String</span><span class="sxs-lookup"><span data-stu-id="aa0d2-117">String</span></span>|<span data-ttu-id="aa0d2-118">O nome do arquivo ou pasta para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="aa0d2-118">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="aa0d2-119">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="aa0d2-119">check32BitOn64System</span></span>|<span data-ttu-id="aa0d2-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa0d2-120">Boolean</span></span>|<span data-ttu-id="aa0d2-121">Um valor que indica se este arquivo ou pasta é para verificar o aplicativo de 32 bits no sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="aa0d2-121">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="aa0d2-122">Detecção</span><span class="sxs-lookup"><span data-stu-id="aa0d2-122">detectionType</span></span>|[<span data-ttu-id="aa0d2-123">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="aa0d2-123">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="aa0d2-124">O tipo de detecção do sistema de arquivos.</span><span class="sxs-lookup"><span data-stu-id="aa0d2-124">The file system detection type.</span></span> <span data-ttu-id="aa0d2-125">Os valores possíveis são: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span><span class="sxs-lookup"><span data-stu-id="aa0d2-125">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|
|<span data-ttu-id="aa0d2-126">operator</span><span class="sxs-lookup"><span data-stu-id="aa0d2-126">operator</span></span>|[<span data-ttu-id="aa0d2-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="aa0d2-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="aa0d2-128">O operador para detecção de arquivo ou pasta.</span><span class="sxs-lookup"><span data-stu-id="aa0d2-128">The operator for file or folder detection.</span></span> <span data-ttu-id="aa0d2-129">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="aa0d2-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="aa0d2-130">detecçaovalue</span><span class="sxs-lookup"><span data-stu-id="aa0d2-130">detectionValue</span></span>|<span data-ttu-id="aa0d2-131">String</span><span class="sxs-lookup"><span data-stu-id="aa0d2-131">String</span></span>|<span data-ttu-id="aa0d2-132">O valor de detecção de arquivo ou pasta</span><span class="sxs-lookup"><span data-stu-id="aa0d2-132">The file or folder detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa0d2-133">Relações</span><span class="sxs-lookup"><span data-stu-id="aa0d2-133">Relationships</span></span>
<span data-ttu-id="aa0d2-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aa0d2-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa0d2-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aa0d2-135">JSON Representation</span></span>
<span data-ttu-id="aa0d2-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aa0d2-136">Here is a JSON representation of the resource.</span></span>
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





