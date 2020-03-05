---
title: tipo de recurso win32LobAppFileSystemRequirement
description: Contém um caminho de arquivo ou pasta para detectar um aplicativo Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: aa42d12dca0c019febaa35ca70aebfb37d6c7597
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42490704"
---
# <a name="win32lobappfilesystemrequirement-resource-type"></a><span data-ttu-id="3f7f2-103">tipo de recurso win32LobAppFileSystemRequirement</span><span class="sxs-lookup"><span data-stu-id="3f7f2-103">win32LobAppFileSystemRequirement resource type</span></span>

<span data-ttu-id="3f7f2-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3f7f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f7f2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3f7f2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f7f2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3f7f2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f7f2-107">Contém um caminho de arquivo ou pasta para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="3f7f2-107">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="3f7f2-108">Herda de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="3f7f2-108">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3f7f2-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3f7f2-109">Properties</span></span>
|<span data-ttu-id="3f7f2-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f7f2-110">Property</span></span>|<span data-ttu-id="3f7f2-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f7f2-111">Type</span></span>|<span data-ttu-id="3f7f2-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f7f2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f7f2-113">operator</span><span class="sxs-lookup"><span data-stu-id="3f7f2-113">operator</span></span>|[<span data-ttu-id="3f7f2-114">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="3f7f2-114">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="3f7f2-115">O operador para detecção herdada de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span><span class="sxs-lookup"><span data-stu-id="3f7f2-115">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="3f7f2-116">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="3f7f2-116">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="3f7f2-117">detecçaovalue</span><span class="sxs-lookup"><span data-stu-id="3f7f2-117">detectionValue</span></span>|<span data-ttu-id="3f7f2-118">String</span><span class="sxs-lookup"><span data-stu-id="3f7f2-118">String</span></span>|<span data-ttu-id="3f7f2-119">O valor de detecção herdado de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="3f7f2-119">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="3f7f2-120">caminho</span><span class="sxs-lookup"><span data-stu-id="3f7f2-120">path</span></span>|<span data-ttu-id="3f7f2-121">String</span><span class="sxs-lookup"><span data-stu-id="3f7f2-121">String</span></span>|<span data-ttu-id="3f7f2-122">O caminho do arquivo ou da pasta para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="3f7f2-122">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="3f7f2-123">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="3f7f2-123">fileOrFolderName</span></span>|<span data-ttu-id="3f7f2-124">String</span><span class="sxs-lookup"><span data-stu-id="3f7f2-124">String</span></span>|<span data-ttu-id="3f7f2-125">O nome do arquivo ou pasta para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="3f7f2-125">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="3f7f2-126">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="3f7f2-126">check32BitOn64System</span></span>|<span data-ttu-id="3f7f2-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f7f2-127">Boolean</span></span>|<span data-ttu-id="3f7f2-128">Um valor que indica se este arquivo ou pasta é para verificar o aplicativo de 32 bits no sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="3f7f2-128">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="3f7f2-129">Detecção</span><span class="sxs-lookup"><span data-stu-id="3f7f2-129">detectionType</span></span>|[<span data-ttu-id="3f7f2-130">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="3f7f2-130">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="3f7f2-131">O tipo de detecção do sistema de arquivos.</span><span class="sxs-lookup"><span data-stu-id="3f7f2-131">The file system detection type.</span></span> <span data-ttu-id="3f7f2-132">Os valores possíveis são: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span><span class="sxs-lookup"><span data-stu-id="3f7f2-132">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f7f2-133">Relações</span><span class="sxs-lookup"><span data-stu-id="3f7f2-133">Relationships</span></span>
<span data-ttu-id="3f7f2-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3f7f2-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f7f2-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3f7f2-135">JSON Representation</span></span>
<span data-ttu-id="3f7f2-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3f7f2-136">Here is a JSON representation of the resource.</span></span>
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



