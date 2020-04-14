---
title: tipo de recurso win32LobAppFileSystemRequirement
description: Contém um caminho de arquivo ou pasta para detectar um aplicativo Win32
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f32327461274585941779c45aa7dc2b485acf12f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422985"
---
# <a name="win32lobappfilesystemrequirement-resource-type"></a><span data-ttu-id="f5657-103">tipo de recurso win32LobAppFileSystemRequirement</span><span class="sxs-lookup"><span data-stu-id="f5657-103">win32LobAppFileSystemRequirement resource type</span></span>

<span data-ttu-id="f5657-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5657-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5657-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f5657-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5657-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f5657-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5657-107">Contém um caminho de arquivo ou pasta para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="f5657-107">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="f5657-108">Herda de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="f5657-108">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f5657-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f5657-109">Properties</span></span>
|<span data-ttu-id="f5657-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5657-110">Property</span></span>|<span data-ttu-id="f5657-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5657-111">Type</span></span>|<span data-ttu-id="f5657-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5657-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5657-113">operator</span><span class="sxs-lookup"><span data-stu-id="f5657-113">operator</span></span>|[<span data-ttu-id="f5657-114">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="f5657-114">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="f5657-115">O operador para detecção herdada de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span><span class="sxs-lookup"><span data-stu-id="f5657-115">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="f5657-116">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="f5657-116">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="f5657-117">detecçaovalue</span><span class="sxs-lookup"><span data-stu-id="f5657-117">detectionValue</span></span>|<span data-ttu-id="f5657-118">String</span><span class="sxs-lookup"><span data-stu-id="f5657-118">String</span></span>|<span data-ttu-id="f5657-119">O valor de detecção herdado de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="f5657-119">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="f5657-120">caminho</span><span class="sxs-lookup"><span data-stu-id="f5657-120">path</span></span>|<span data-ttu-id="f5657-121">String</span><span class="sxs-lookup"><span data-stu-id="f5657-121">String</span></span>|<span data-ttu-id="f5657-122">O caminho do arquivo ou da pasta para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="f5657-122">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="f5657-123">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="f5657-123">fileOrFolderName</span></span>|<span data-ttu-id="f5657-124">String</span><span class="sxs-lookup"><span data-stu-id="f5657-124">String</span></span>|<span data-ttu-id="f5657-125">O nome do arquivo ou pasta para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="f5657-125">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="f5657-126">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="f5657-126">check32BitOn64System</span></span>|<span data-ttu-id="f5657-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5657-127">Boolean</span></span>|<span data-ttu-id="f5657-128">Um valor que indica se este arquivo ou pasta é para verificar o aplicativo de 32 bits no sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="f5657-128">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="f5657-129">Detecção</span><span class="sxs-lookup"><span data-stu-id="f5657-129">detectionType</span></span>|[<span data-ttu-id="f5657-130">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="f5657-130">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="f5657-131">O tipo de detecção do sistema de arquivos.</span><span class="sxs-lookup"><span data-stu-id="f5657-131">The file system detection type.</span></span> <span data-ttu-id="f5657-132">Os valores possíveis são: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span><span class="sxs-lookup"><span data-stu-id="f5657-132">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5657-133">Relações</span><span class="sxs-lookup"><span data-stu-id="f5657-133">Relationships</span></span>
<span data-ttu-id="f5657-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f5657-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5657-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f5657-135">JSON Representation</span></span>
<span data-ttu-id="f5657-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f5657-136">Here is a JSON representation of the resource.</span></span>
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



