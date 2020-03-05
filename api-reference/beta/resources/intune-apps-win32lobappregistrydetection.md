---
title: tipo de recurso win32LobAppRegistryDetection
description: Contém as propriedades do registro para detectar um aplicativo Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: da9f63d4a16df728320e0f3144bee32ad90f2922
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42490459"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="25417-103">tipo de recurso win32LobAppRegistryDetection</span><span class="sxs-lookup"><span data-stu-id="25417-103">win32LobAppRegistryDetection resource type</span></span>

<span data-ttu-id="25417-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="25417-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25417-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="25417-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25417-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="25417-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25417-107">Contém as propriedades do registro para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="25417-107">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="25417-108">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="25417-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="25417-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="25417-109">Properties</span></span>
|<span data-ttu-id="25417-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25417-110">Property</span></span>|<span data-ttu-id="25417-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="25417-111">Type</span></span>|<span data-ttu-id="25417-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="25417-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25417-113">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="25417-113">check32BitOn64System</span></span>|<span data-ttu-id="25417-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="25417-114">Boolean</span></span>|<span data-ttu-id="25417-115">Um valor que indica se este caminho de registro é para verificar o aplicativo de 32 bits no sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="25417-115">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="25417-116">Caminho-chave</span><span class="sxs-lookup"><span data-stu-id="25417-116">keyPath</span></span>|<span data-ttu-id="25417-117">String</span><span class="sxs-lookup"><span data-stu-id="25417-117">String</span></span>|<span data-ttu-id="25417-118">O caminho da chave do registro para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="25417-118">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="25417-119">valueName</span><span class="sxs-lookup"><span data-stu-id="25417-119">valueName</span></span>|<span data-ttu-id="25417-120">String</span><span class="sxs-lookup"><span data-stu-id="25417-120">String</span></span>|<span data-ttu-id="25417-121">O nome do valor do registro</span><span class="sxs-lookup"><span data-stu-id="25417-121">The registry value name</span></span>|
|<span data-ttu-id="25417-122">Detecção</span><span class="sxs-lookup"><span data-stu-id="25417-122">detectionType</span></span>|[<span data-ttu-id="25417-123">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="25417-123">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="25417-124">O tipo de detecção de dados do registro.</span><span class="sxs-lookup"><span data-stu-id="25417-124">The registry data detection type.</span></span> <span data-ttu-id="25417-125">Os possíveis valores são: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="25417-125">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="25417-126">operator</span><span class="sxs-lookup"><span data-stu-id="25417-126">operator</span></span>|[<span data-ttu-id="25417-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="25417-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="25417-128">O operador para a detecção de dados do registro.</span><span class="sxs-lookup"><span data-stu-id="25417-128">The operator for registry data detection.</span></span> <span data-ttu-id="25417-129">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="25417-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="25417-130">detecçaovalue</span><span class="sxs-lookup"><span data-stu-id="25417-130">detectionValue</span></span>|<span data-ttu-id="25417-131">String</span><span class="sxs-lookup"><span data-stu-id="25417-131">String</span></span>|<span data-ttu-id="25417-132">O valor de detecção do registro</span><span class="sxs-lookup"><span data-stu-id="25417-132">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="25417-133">Relações</span><span class="sxs-lookup"><span data-stu-id="25417-133">Relationships</span></span>
<span data-ttu-id="25417-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="25417-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="25417-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="25417-135">JSON Representation</span></span>
<span data-ttu-id="25417-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="25417-136">Here is a JSON representation of the resource.</span></span>
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



