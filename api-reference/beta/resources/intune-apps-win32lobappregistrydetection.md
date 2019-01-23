---
title: tipo de recurso de win32LobAppRegistryDetection
description: Contém propriedades do registro para detectar um aplicativo Win32
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bb10a96a14d3c26503b33191fbb3c1b883245da7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402661"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="8d6ac-103">tipo de recurso de win32LobAppRegistryDetection</span><span class="sxs-lookup"><span data-stu-id="8d6ac-103">win32LobAppRegistryDetection resource type</span></span>

> <span data-ttu-id="8d6ac-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="8d6ac-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8d6ac-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8d6ac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8d6ac-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="8d6ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d6ac-107">Contém propriedades do registro para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="8d6ac-107">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="8d6ac-108">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="8d6ac-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8d6ac-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8d6ac-109">Properties</span></span>
|<span data-ttu-id="8d6ac-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d6ac-110">Property</span></span>|<span data-ttu-id="8d6ac-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d6ac-111">Type</span></span>|<span data-ttu-id="8d6ac-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d6ac-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d6ac-113">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="8d6ac-113">check32BitOn64System</span></span>|<span data-ttu-id="8d6ac-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d6ac-114">Boolean</span></span>|<span data-ttu-id="8d6ac-115">Um valor indicando se nesse caminho do registro é para verificação de aplicativo de 32 bits no sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="8d6ac-115">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="8d6ac-116">caminho-chave</span><span class="sxs-lookup"><span data-stu-id="8d6ac-116">keyPath</span></span>|<span data-ttu-id="8d6ac-117">String</span><span class="sxs-lookup"><span data-stu-id="8d6ac-117">String</span></span>|<span data-ttu-id="8d6ac-118">O caminho da chave do registro para detectar app Win32 linha de negócios (LoB)</span><span class="sxs-lookup"><span data-stu-id="8d6ac-118">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="8d6ac-119">valueName</span><span class="sxs-lookup"><span data-stu-id="8d6ac-119">valueName</span></span>|<span data-ttu-id="8d6ac-120">String</span><span class="sxs-lookup"><span data-stu-id="8d6ac-120">String</span></span>|<span data-ttu-id="8d6ac-121">O nome do valor do registro</span><span class="sxs-lookup"><span data-stu-id="8d6ac-121">The registry value name</span></span>|
|<span data-ttu-id="8d6ac-122">tipo de detecção</span><span class="sxs-lookup"><span data-stu-id="8d6ac-122">detectionType</span></span>|[<span data-ttu-id="8d6ac-123">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="8d6ac-123">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="8d6ac-124">O tipo de detecção de dados de registro.</span><span class="sxs-lookup"><span data-stu-id="8d6ac-124">The registry data detection type.</span></span> <span data-ttu-id="8d6ac-125">Os possíveis valores são: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="8d6ac-125">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="8d6ac-126">operador</span><span class="sxs-lookup"><span data-stu-id="8d6ac-126">operator</span></span>|[<span data-ttu-id="8d6ac-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="8d6ac-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="8d6ac-128">O operador para detecção de dados de registro.</span><span class="sxs-lookup"><span data-stu-id="8d6ac-128">The operator for registry data detection.</span></span> <span data-ttu-id="8d6ac-129">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="8d6ac-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="8d6ac-130">detectionValue</span><span class="sxs-lookup"><span data-stu-id="8d6ac-130">detectionValue</span></span>|<span data-ttu-id="8d6ac-131">String</span><span class="sxs-lookup"><span data-stu-id="8d6ac-131">String</span></span>|<span data-ttu-id="8d6ac-132">O valor de detecção do registro</span><span class="sxs-lookup"><span data-stu-id="8d6ac-132">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d6ac-133">Relações</span><span class="sxs-lookup"><span data-stu-id="8d6ac-133">Relationships</span></span>
<span data-ttu-id="8d6ac-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8d6ac-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d6ac-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8d6ac-135">JSON Representation</span></span>
<span data-ttu-id="8d6ac-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8d6ac-136">Here is a JSON representation of the resource.</span></span>
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




