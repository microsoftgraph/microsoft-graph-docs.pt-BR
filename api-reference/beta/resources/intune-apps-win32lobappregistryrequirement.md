---
title: tipo de recurso win32LobAppRegistryRequirement
description: Contém as propriedades do registro para detectar um aplicativo Win32
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 032300f73b249603c36d846db54b39ef050d6e69
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797567"
---
# <a name="win32lobappregistryrequirement-resource-type"></a><span data-ttu-id="52e01-103">tipo de recurso win32LobAppRegistryRequirement</span><span class="sxs-lookup"><span data-stu-id="52e01-103">win32LobAppRegistryRequirement resource type</span></span>

> <span data-ttu-id="52e01-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="52e01-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52e01-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="52e01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52e01-106">Contém as propriedades do registro para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="52e01-106">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="52e01-107">Herda de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="52e01-107">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="52e01-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52e01-108">Properties</span></span>
|<span data-ttu-id="52e01-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52e01-109">Property</span></span>|<span data-ttu-id="52e01-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="52e01-110">Type</span></span>|<span data-ttu-id="52e01-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="52e01-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52e01-112">operator</span><span class="sxs-lookup"><span data-stu-id="52e01-112">operator</span></span>|[<span data-ttu-id="52e01-113">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="52e01-113">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="52e01-114">O operador para detecção herdada de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span><span class="sxs-lookup"><span data-stu-id="52e01-114">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="52e01-115">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="52e01-115">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="52e01-116">detecçaovalue</span><span class="sxs-lookup"><span data-stu-id="52e01-116">detectionValue</span></span>|<span data-ttu-id="52e01-117">String</span><span class="sxs-lookup"><span data-stu-id="52e01-117">String</span></span>|<span data-ttu-id="52e01-118">O valor de detecção herdado de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="52e01-118">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="52e01-119">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="52e01-119">check32BitOn64System</span></span>|<span data-ttu-id="52e01-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="52e01-120">Boolean</span></span>|<span data-ttu-id="52e01-121">Um valor que indica se este caminho de registro é para verificar o aplicativo de 32 bits no sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="52e01-121">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="52e01-122">Caminho-chave</span><span class="sxs-lookup"><span data-stu-id="52e01-122">keyPath</span></span>|<span data-ttu-id="52e01-123">String</span><span class="sxs-lookup"><span data-stu-id="52e01-123">String</span></span>|<span data-ttu-id="52e01-124">O caminho da chave do registro para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="52e01-124">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="52e01-125">valueName</span><span class="sxs-lookup"><span data-stu-id="52e01-125">valueName</span></span>|<span data-ttu-id="52e01-126">String</span><span class="sxs-lookup"><span data-stu-id="52e01-126">String</span></span>|<span data-ttu-id="52e01-127">O nome do valor do registro</span><span class="sxs-lookup"><span data-stu-id="52e01-127">The registry value name</span></span>|
|<span data-ttu-id="52e01-128">Detecção</span><span class="sxs-lookup"><span data-stu-id="52e01-128">detectionType</span></span>|[<span data-ttu-id="52e01-129">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="52e01-129">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="52e01-130">O tipo de detecção de dados do registro.</span><span class="sxs-lookup"><span data-stu-id="52e01-130">The registry data detection type.</span></span> <span data-ttu-id="52e01-131">Os possíveis valores são: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="52e01-131">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52e01-132">Relações</span><span class="sxs-lookup"><span data-stu-id="52e01-132">Relationships</span></span>
<span data-ttu-id="52e01-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="52e01-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="52e01-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52e01-134">JSON Representation</span></span>
<span data-ttu-id="52e01-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52e01-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRegistryRequirement",
  "operator": "String",
  "detectionValue": "String",
  "check32BitOn64System": true,
  "keyPath": "String",
  "valueName": "String",
  "detectionType": "String"
}
```



