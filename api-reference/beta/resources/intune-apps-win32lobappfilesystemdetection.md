---
title: tipo de recurso de win32LobAppFileSystemDetection
description: Contém o caminho de arquivo ou pasta para detectar um aplicativo Win32
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b5fb4e66ce17fb7a964f3210244e2f3a7027c578
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415226"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a><span data-ttu-id="af6ee-103">tipo de recurso de win32LobAppFileSystemDetection</span><span class="sxs-lookup"><span data-stu-id="af6ee-103">win32LobAppFileSystemDetection resource type</span></span>

> <span data-ttu-id="af6ee-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="af6ee-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="af6ee-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="af6ee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="af6ee-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="af6ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af6ee-107">Contém o caminho de arquivo ou pasta para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="af6ee-107">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="af6ee-108">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="af6ee-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="af6ee-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="af6ee-109">Properties</span></span>
|<span data-ttu-id="af6ee-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af6ee-110">Property</span></span>|<span data-ttu-id="af6ee-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="af6ee-111">Type</span></span>|<span data-ttu-id="af6ee-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="af6ee-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af6ee-113">caminho</span><span class="sxs-lookup"><span data-stu-id="af6ee-113">path</span></span>|<span data-ttu-id="af6ee-114">String</span><span class="sxs-lookup"><span data-stu-id="af6ee-114">String</span></span>|<span data-ttu-id="af6ee-115">O caminho de arquivo ou pasta para detectar app Win32 linha de negócios (LoB)</span><span class="sxs-lookup"><span data-stu-id="af6ee-115">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="af6ee-116">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="af6ee-116">fileOrFolderName</span></span>|<span data-ttu-id="af6ee-117">String</span><span class="sxs-lookup"><span data-stu-id="af6ee-117">String</span></span>|<span data-ttu-id="af6ee-118">O nome de arquivo ou pasta para detectar app Win32 linha de negócios (LoB)</span><span class="sxs-lookup"><span data-stu-id="af6ee-118">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="af6ee-119">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="af6ee-119">check32BitOn64System</span></span>|<span data-ttu-id="af6ee-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="af6ee-120">Boolean</span></span>|<span data-ttu-id="af6ee-121">Um valor que indica se este arquivo ou pasta é para verificar o aplicativo de 32 bits no sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="af6ee-121">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="af6ee-122">tipo de detecção</span><span class="sxs-lookup"><span data-stu-id="af6ee-122">detectionType</span></span>|[<span data-ttu-id="af6ee-123">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="af6ee-123">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="af6ee-124">O tipo de detecção de sistema de arquivos.</span><span class="sxs-lookup"><span data-stu-id="af6ee-124">The file system detection type.</span></span> <span data-ttu-id="af6ee-125">Os possíveis valores são: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.</span><span class="sxs-lookup"><span data-stu-id="af6ee-125">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.</span></span>|
|<span data-ttu-id="af6ee-126">operador</span><span class="sxs-lookup"><span data-stu-id="af6ee-126">operator</span></span>|[<span data-ttu-id="af6ee-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="af6ee-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="af6ee-128">O operador para detecção de arquivo ou fodler.</span><span class="sxs-lookup"><span data-stu-id="af6ee-128">The operator for file or fodler detection.</span></span> <span data-ttu-id="af6ee-129">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="af6ee-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="af6ee-130">detectionValue</span><span class="sxs-lookup"><span data-stu-id="af6ee-130">detectionValue</span></span>|<span data-ttu-id="af6ee-131">String</span><span class="sxs-lookup"><span data-stu-id="af6ee-131">String</span></span>|<span data-ttu-id="af6ee-132">O valor de detecção de arquivo ou pasta</span><span class="sxs-lookup"><span data-stu-id="af6ee-132">The file or folder detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="af6ee-133">Relações</span><span class="sxs-lookup"><span data-stu-id="af6ee-133">Relationships</span></span>
<span data-ttu-id="af6ee-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="af6ee-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="af6ee-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="af6ee-135">JSON Representation</span></span>
<span data-ttu-id="af6ee-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="af6ee-136">Here is a JSON representation of the resource.</span></span>
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




