---
title: tipo de recurso win32LobAppFileSystemRequirement
description: Contém um caminho de arquivo ou pasta para detectar um aplicativo Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ab011739ed24a0f9880ccc72461f0c4eef5c0655
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708974"
---
# <a name="win32lobappfilesystemrequirement-resource-type"></a><span data-ttu-id="d34b4-103">tipo de recurso win32LobAppFileSystemRequirement</span><span class="sxs-lookup"><span data-stu-id="d34b4-103">win32LobAppFileSystemRequirement resource type</span></span>

<span data-ttu-id="d34b4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d34b4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d34b4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d34b4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d34b4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d34b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d34b4-107">Contém um caminho de arquivo ou pasta para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="d34b4-107">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="d34b4-108">Herda de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="d34b4-108">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d34b4-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d34b4-109">Properties</span></span>
|<span data-ttu-id="d34b4-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d34b4-110">Property</span></span>|<span data-ttu-id="d34b4-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d34b4-111">Type</span></span>|<span data-ttu-id="d34b4-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d34b4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d34b4-113">operator</span><span class="sxs-lookup"><span data-stu-id="d34b4-113">operator</span></span>|[<span data-ttu-id="d34b4-114">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="d34b4-114">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="d34b4-115">O operador para detecção herdada de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span><span class="sxs-lookup"><span data-stu-id="d34b4-115">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="d34b4-116">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="d34b4-116">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="d34b4-117">detecçaovalue</span><span class="sxs-lookup"><span data-stu-id="d34b4-117">detectionValue</span></span>|<span data-ttu-id="d34b4-118">String</span><span class="sxs-lookup"><span data-stu-id="d34b4-118">String</span></span>|<span data-ttu-id="d34b4-119">O valor de detecção herdado de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="d34b4-119">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="d34b4-120">caminho</span><span class="sxs-lookup"><span data-stu-id="d34b4-120">path</span></span>|<span data-ttu-id="d34b4-121">String</span><span class="sxs-lookup"><span data-stu-id="d34b4-121">String</span></span>|<span data-ttu-id="d34b4-122">O caminho do arquivo ou da pasta para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="d34b4-122">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="d34b4-123">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="d34b4-123">fileOrFolderName</span></span>|<span data-ttu-id="d34b4-124">String</span><span class="sxs-lookup"><span data-stu-id="d34b4-124">String</span></span>|<span data-ttu-id="d34b4-125">O nome do arquivo ou pasta para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="d34b4-125">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="d34b4-126">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="d34b4-126">check32BitOn64System</span></span>|<span data-ttu-id="d34b4-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="d34b4-127">Boolean</span></span>|<span data-ttu-id="d34b4-128">Um valor que indica se este arquivo ou pasta é para verificar o aplicativo de 32 bits no sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="d34b4-128">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="d34b4-129">Detecção</span><span class="sxs-lookup"><span data-stu-id="d34b4-129">detectionType</span></span>|[<span data-ttu-id="d34b4-130">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="d34b4-130">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="d34b4-131">O tipo de detecção do sistema de arquivos.</span><span class="sxs-lookup"><span data-stu-id="d34b4-131">The file system detection type.</span></span> <span data-ttu-id="d34b4-132">Os valores possíveis são: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span><span class="sxs-lookup"><span data-stu-id="d34b4-132">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d34b4-133">Relações</span><span class="sxs-lookup"><span data-stu-id="d34b4-133">Relationships</span></span>
<span data-ttu-id="d34b4-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d34b4-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d34b4-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d34b4-135">JSON Representation</span></span>
<span data-ttu-id="d34b4-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d34b4-136">Here is a JSON representation of the resource.</span></span>
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





