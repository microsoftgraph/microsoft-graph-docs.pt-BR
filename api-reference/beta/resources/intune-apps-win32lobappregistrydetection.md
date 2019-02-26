---
title: tipo de recurso win32LobAppRegistryDetection
description: Contém as propriedades do registro para detectar um aplicativo Win32
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 076251ea185359127c3dad3610ec944f7cdb3178
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169542"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="85de3-103">tipo de recurso win32LobAppRegistryDetection</span><span class="sxs-lookup"><span data-stu-id="85de3-103">win32LobAppRegistryDetection resource type</span></span>

> <span data-ttu-id="85de3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="85de3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85de3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="85de3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85de3-106">Contém as propriedades do registro para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="85de3-106">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="85de3-107">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="85de3-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="85de3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="85de3-108">Properties</span></span>
|<span data-ttu-id="85de3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85de3-109">Property</span></span>|<span data-ttu-id="85de3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="85de3-110">Type</span></span>|<span data-ttu-id="85de3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="85de3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85de3-112">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="85de3-112">check32BitOn64System</span></span>|<span data-ttu-id="85de3-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="85de3-113">Boolean</span></span>|<span data-ttu-id="85de3-114">Um valor que indica se este caminho de registro é para verificar o aplicativo de 32 bits no sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="85de3-114">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="85de3-115">Caminho-chave</span><span class="sxs-lookup"><span data-stu-id="85de3-115">keyPath</span></span>|<span data-ttu-id="85de3-116">String</span><span class="sxs-lookup"><span data-stu-id="85de3-116">String</span></span>|<span data-ttu-id="85de3-117">O caminho da chave do registro para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="85de3-117">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="85de3-118">valueName</span><span class="sxs-lookup"><span data-stu-id="85de3-118">valueName</span></span>|<span data-ttu-id="85de3-119">String</span><span class="sxs-lookup"><span data-stu-id="85de3-119">String</span></span>|<span data-ttu-id="85de3-120">O nome do valor do registro</span><span class="sxs-lookup"><span data-stu-id="85de3-120">The registry value name</span></span>|
|<span data-ttu-id="85de3-121">Detecção</span><span class="sxs-lookup"><span data-stu-id="85de3-121">detectionType</span></span>|[<span data-ttu-id="85de3-122">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="85de3-122">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="85de3-123">O tipo de detecção de dados do registro.</span><span class="sxs-lookup"><span data-stu-id="85de3-123">The registry data detection type.</span></span> <span data-ttu-id="85de3-124">Os possíveis valores são: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="85de3-124">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="85de3-125">operador</span><span class="sxs-lookup"><span data-stu-id="85de3-125">operator</span></span>|[<span data-ttu-id="85de3-126">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="85de3-126">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="85de3-127">O operador para a detecção de dados do registro.</span><span class="sxs-lookup"><span data-stu-id="85de3-127">The operator for registry data detection.</span></span> <span data-ttu-id="85de3-128">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="85de3-128">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="85de3-129">detecçaovalue</span><span class="sxs-lookup"><span data-stu-id="85de3-129">detectionValue</span></span>|<span data-ttu-id="85de3-130">String</span><span class="sxs-lookup"><span data-stu-id="85de3-130">String</span></span>|<span data-ttu-id="85de3-131">O valor de detecção do registro</span><span class="sxs-lookup"><span data-stu-id="85de3-131">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="85de3-132">Relações</span><span class="sxs-lookup"><span data-stu-id="85de3-132">Relationships</span></span>
<span data-ttu-id="85de3-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="85de3-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="85de3-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="85de3-134">JSON Representation</span></span>
<span data-ttu-id="85de3-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="85de3-135">Here is a JSON representation of the resource.</span></span>
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




