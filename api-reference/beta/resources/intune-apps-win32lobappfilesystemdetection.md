---
title: tipo de recurso de win32LobAppFileSystemDetection
description: Contém o caminho de arquivo ou pasta para detectar um aplicativo Win32
author: tfitzmac
ms.openlocfilehash: 26d65c8a1fcf70032c780b3e6e00a198a8ff2c30
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306871"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a><span data-ttu-id="20dce-103">tipo de recurso de win32LobAppFileSystemDetection</span><span class="sxs-lookup"><span data-stu-id="20dce-103">win32LobAppFileSystemDetection resource type</span></span>

> <span data-ttu-id="20dce-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="20dce-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20dce-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="20dce-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="20dce-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="20dce-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20dce-107">Contém o caminho de arquivo ou pasta para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="20dce-107">Contains file or folder path to detect a Win32 App</span></span>

<span data-ttu-id="20dce-108">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="20dce-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="20dce-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20dce-109">Properties</span></span>
|<span data-ttu-id="20dce-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20dce-110">Property</span></span>|<span data-ttu-id="20dce-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="20dce-111">Type</span></span>|<span data-ttu-id="20dce-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="20dce-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20dce-113">caminho</span><span class="sxs-lookup"><span data-stu-id="20dce-113">path</span></span>|<span data-ttu-id="20dce-114">String</span><span class="sxs-lookup"><span data-stu-id="20dce-114">String</span></span>|<span data-ttu-id="20dce-115">O caminho de arquivo ou pasta para detectar app Win32 linha de negócios (LoB)</span><span class="sxs-lookup"><span data-stu-id="20dce-115">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="20dce-116">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="20dce-116">fileOrFolderName</span></span>|<span data-ttu-id="20dce-117">String</span><span class="sxs-lookup"><span data-stu-id="20dce-117">String</span></span>|<span data-ttu-id="20dce-118">O nome de arquivo ou pasta para detectar app Win32 linha de negócios (LoB)</span><span class="sxs-lookup"><span data-stu-id="20dce-118">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="20dce-119">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="20dce-119">check32BitOn64System</span></span>|<span data-ttu-id="20dce-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="20dce-120">Boolean</span></span>|<span data-ttu-id="20dce-121">Um valor que indica se este arquivo ou pasta é para verificar o aplicativo de 32 bits no sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="20dce-121">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="20dce-122">tipo de detecção</span><span class="sxs-lookup"><span data-stu-id="20dce-122">detectionType</span></span>|[<span data-ttu-id="20dce-123">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="20dce-123">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="20dce-124">O tipo de detecção de sistema de arquivos.</span><span class="sxs-lookup"><span data-stu-id="20dce-124">The file system detection type.</span></span> <span data-ttu-id="20dce-125">Os possíveis valores são: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.</span><span class="sxs-lookup"><span data-stu-id="20dce-125">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.</span></span>|
|<span data-ttu-id="20dce-126">operador</span><span class="sxs-lookup"><span data-stu-id="20dce-126">operator</span></span>|[<span data-ttu-id="20dce-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="20dce-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="20dce-128">O operador para detecção de arquivo ou fodler.</span><span class="sxs-lookup"><span data-stu-id="20dce-128">The operator for file or fodler detection.</span></span> <span data-ttu-id="20dce-129">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="20dce-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="20dce-130">detectionValue</span><span class="sxs-lookup"><span data-stu-id="20dce-130">detectionValue</span></span>|<span data-ttu-id="20dce-131">String</span><span class="sxs-lookup"><span data-stu-id="20dce-131">String</span></span>|<span data-ttu-id="20dce-132">O valor de detecção de arquivo ou pasta</span><span class="sxs-lookup"><span data-stu-id="20dce-132">The file or folder detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="20dce-133">Relações</span><span class="sxs-lookup"><span data-stu-id="20dce-133">Relationships</span></span>
<span data-ttu-id="20dce-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="20dce-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="20dce-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="20dce-135">JSON Representation</span></span>
<span data-ttu-id="20dce-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="20dce-136">Here is a JSON representation of the resource.</span></span>
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





