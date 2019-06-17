---
title: tipo de recurso win32LobAppRegistryDetection
description: Contém as propriedades do registro para detectar um aplicativo Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3013ca82a0545379c96cf832818783dedd4576f4
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34986099"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="732e9-103">tipo de recurso win32LobAppRegistryDetection</span><span class="sxs-lookup"><span data-stu-id="732e9-103">win32LobAppRegistryDetection resource type</span></span>

> <span data-ttu-id="732e9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="732e9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="732e9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="732e9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="732e9-106">Contém as propriedades do registro para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="732e9-106">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="732e9-107">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="732e9-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="732e9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="732e9-108">Properties</span></span>
|<span data-ttu-id="732e9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="732e9-109">Property</span></span>|<span data-ttu-id="732e9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="732e9-110">Type</span></span>|<span data-ttu-id="732e9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="732e9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="732e9-112">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="732e9-112">check32BitOn64System</span></span>|<span data-ttu-id="732e9-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="732e9-113">Boolean</span></span>|<span data-ttu-id="732e9-114">Um valor que indica se este caminho de registro é para verificar o aplicativo de 32 bits no sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="732e9-114">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="732e9-115">Caminho-chave</span><span class="sxs-lookup"><span data-stu-id="732e9-115">keyPath</span></span>|<span data-ttu-id="732e9-116">String</span><span class="sxs-lookup"><span data-stu-id="732e9-116">String</span></span>|<span data-ttu-id="732e9-117">O caminho da chave do registro para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="732e9-117">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="732e9-118">valueName</span><span class="sxs-lookup"><span data-stu-id="732e9-118">valueName</span></span>|<span data-ttu-id="732e9-119">String</span><span class="sxs-lookup"><span data-stu-id="732e9-119">String</span></span>|<span data-ttu-id="732e9-120">O nome do valor do registro</span><span class="sxs-lookup"><span data-stu-id="732e9-120">The registry value name</span></span>|
|<span data-ttu-id="732e9-121">Detecção</span><span class="sxs-lookup"><span data-stu-id="732e9-121">detectionType</span></span>|[<span data-ttu-id="732e9-122">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="732e9-122">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="732e9-123">O tipo de detecção de dados do registro.</span><span class="sxs-lookup"><span data-stu-id="732e9-123">The registry data detection type.</span></span> <span data-ttu-id="732e9-124">Os possíveis valores são: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="732e9-124">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="732e9-125">operator</span><span class="sxs-lookup"><span data-stu-id="732e9-125">operator</span></span>|[<span data-ttu-id="732e9-126">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="732e9-126">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="732e9-127">O operador para a detecção de dados do registro.</span><span class="sxs-lookup"><span data-stu-id="732e9-127">The operator for registry data detection.</span></span> <span data-ttu-id="732e9-128">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="732e9-128">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="732e9-129">detecçaovalue</span><span class="sxs-lookup"><span data-stu-id="732e9-129">detectionValue</span></span>|<span data-ttu-id="732e9-130">String</span><span class="sxs-lookup"><span data-stu-id="732e9-130">String</span></span>|<span data-ttu-id="732e9-131">O valor de detecção do registro</span><span class="sxs-lookup"><span data-stu-id="732e9-131">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="732e9-132">Relações</span><span class="sxs-lookup"><span data-stu-id="732e9-132">Relationships</span></span>
<span data-ttu-id="732e9-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="732e9-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="732e9-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="732e9-134">JSON Representation</span></span>
<span data-ttu-id="732e9-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="732e9-135">Here is a JSON representation of the resource.</span></span>
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





