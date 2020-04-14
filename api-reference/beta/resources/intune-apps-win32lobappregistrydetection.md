---
title: tipo de recurso win32LobAppRegistryDetection
description: Contém as propriedades do registro para detectar um aplicativo Win32
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2b6f28d6c042ab86273cd11d9e756bb4941e315b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422736"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="50fdd-103">tipo de recurso win32LobAppRegistryDetection</span><span class="sxs-lookup"><span data-stu-id="50fdd-103">win32LobAppRegistryDetection resource type</span></span>

<span data-ttu-id="50fdd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50fdd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50fdd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="50fdd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50fdd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50fdd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50fdd-107">Contém as propriedades do registro para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="50fdd-107">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="50fdd-108">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="50fdd-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="50fdd-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50fdd-109">Properties</span></span>
|<span data-ttu-id="50fdd-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50fdd-110">Property</span></span>|<span data-ttu-id="50fdd-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="50fdd-111">Type</span></span>|<span data-ttu-id="50fdd-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="50fdd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50fdd-113">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="50fdd-113">check32BitOn64System</span></span>|<span data-ttu-id="50fdd-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="50fdd-114">Boolean</span></span>|<span data-ttu-id="50fdd-115">Um valor que indica se este caminho de registro é para verificar o aplicativo de 32 bits no sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="50fdd-115">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="50fdd-116">Caminho-chave</span><span class="sxs-lookup"><span data-stu-id="50fdd-116">keyPath</span></span>|<span data-ttu-id="50fdd-117">String</span><span class="sxs-lookup"><span data-stu-id="50fdd-117">String</span></span>|<span data-ttu-id="50fdd-118">O caminho da chave do registro para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="50fdd-118">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="50fdd-119">valueName</span><span class="sxs-lookup"><span data-stu-id="50fdd-119">valueName</span></span>|<span data-ttu-id="50fdd-120">String</span><span class="sxs-lookup"><span data-stu-id="50fdd-120">String</span></span>|<span data-ttu-id="50fdd-121">O nome do valor do registro</span><span class="sxs-lookup"><span data-stu-id="50fdd-121">The registry value name</span></span>|
|<span data-ttu-id="50fdd-122">Detecção</span><span class="sxs-lookup"><span data-stu-id="50fdd-122">detectionType</span></span>|[<span data-ttu-id="50fdd-123">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="50fdd-123">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="50fdd-124">O tipo de detecção de dados do registro.</span><span class="sxs-lookup"><span data-stu-id="50fdd-124">The registry data detection type.</span></span> <span data-ttu-id="50fdd-125">Os possíveis valores são: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="50fdd-125">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="50fdd-126">operator</span><span class="sxs-lookup"><span data-stu-id="50fdd-126">operator</span></span>|[<span data-ttu-id="50fdd-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="50fdd-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="50fdd-128">O operador para a detecção de dados do registro.</span><span class="sxs-lookup"><span data-stu-id="50fdd-128">The operator for registry data detection.</span></span> <span data-ttu-id="50fdd-129">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="50fdd-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="50fdd-130">detecçaovalue</span><span class="sxs-lookup"><span data-stu-id="50fdd-130">detectionValue</span></span>|<span data-ttu-id="50fdd-131">String</span><span class="sxs-lookup"><span data-stu-id="50fdd-131">String</span></span>|<span data-ttu-id="50fdd-132">O valor de detecção do registro</span><span class="sxs-lookup"><span data-stu-id="50fdd-132">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="50fdd-133">Relações</span><span class="sxs-lookup"><span data-stu-id="50fdd-133">Relationships</span></span>
<span data-ttu-id="50fdd-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="50fdd-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50fdd-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50fdd-135">JSON Representation</span></span>
<span data-ttu-id="50fdd-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="50fdd-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRegistryDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRegistryDetection",
  "check32BitOn64System": true,
  "keyPath": "String",
  "valueName": "String",
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```



