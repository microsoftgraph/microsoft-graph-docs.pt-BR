---
title: tipo de recurso de win32LobAppRegistryDetection
description: Contém propriedades do registro para detectar um aplicativo Win32
author: tfitzmac
ms.openlocfilehash: 5adeca1b569531d15657acc2a8960bab60580dc6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347737"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="afdee-103">tipo de recurso de win32LobAppRegistryDetection</span><span class="sxs-lookup"><span data-stu-id="afdee-103">win32LobAppRegistryDetection resource type</span></span>

> <span data-ttu-id="afdee-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="afdee-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="afdee-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="afdee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="afdee-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="afdee-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="afdee-107">Contém propriedades do registro para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="afdee-107">Contains registry properties to detect a Win32 App</span></span>

<span data-ttu-id="afdee-108">Herda de [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="afdee-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="afdee-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="afdee-109">Properties</span></span>
|<span data-ttu-id="afdee-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="afdee-110">Property</span></span>|<span data-ttu-id="afdee-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="afdee-111">Type</span></span>|<span data-ttu-id="afdee-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="afdee-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afdee-113">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="afdee-113">check32BitOn64System</span></span>|<span data-ttu-id="afdee-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="afdee-114">Boolean</span></span>|<span data-ttu-id="afdee-115">Um valor indicando se nesse caminho do registro é para verificação de aplicativo de 32 bits no sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="afdee-115">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="afdee-116">caminho-chave</span><span class="sxs-lookup"><span data-stu-id="afdee-116">keyPath</span></span>|<span data-ttu-id="afdee-117">String</span><span class="sxs-lookup"><span data-stu-id="afdee-117">String</span></span>|<span data-ttu-id="afdee-118">O caminho da chave do registro para detectar app Win32 linha de negócios (LoB)</span><span class="sxs-lookup"><span data-stu-id="afdee-118">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="afdee-119">valueName</span><span class="sxs-lookup"><span data-stu-id="afdee-119">valueName</span></span>|<span data-ttu-id="afdee-120">String</span><span class="sxs-lookup"><span data-stu-id="afdee-120">String</span></span>|<span data-ttu-id="afdee-121">O nome do valor do registro</span><span class="sxs-lookup"><span data-stu-id="afdee-121">The registry value name</span></span>|
|<span data-ttu-id="afdee-122">tipo de detecção</span><span class="sxs-lookup"><span data-stu-id="afdee-122">detectionType</span></span>|[<span data-ttu-id="afdee-123">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="afdee-123">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="afdee-124">O tipo de detecção de dados de registro.</span><span class="sxs-lookup"><span data-stu-id="afdee-124">The registry data detection type.</span></span> <span data-ttu-id="afdee-125">Os possíveis valores são: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="afdee-125">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="afdee-126">operador</span><span class="sxs-lookup"><span data-stu-id="afdee-126">operator</span></span>|[<span data-ttu-id="afdee-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="afdee-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="afdee-128">O operador para detecção de dados de registro.</span><span class="sxs-lookup"><span data-stu-id="afdee-128">The operator for registry data detection.</span></span> <span data-ttu-id="afdee-129">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="afdee-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="afdee-130">detectionValue</span><span class="sxs-lookup"><span data-stu-id="afdee-130">detectionValue</span></span>|<span data-ttu-id="afdee-131">String</span><span class="sxs-lookup"><span data-stu-id="afdee-131">String</span></span>|<span data-ttu-id="afdee-132">O valor de detecção do registro</span><span class="sxs-lookup"><span data-stu-id="afdee-132">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="afdee-133">Relações</span><span class="sxs-lookup"><span data-stu-id="afdee-133">Relationships</span></span>
<span data-ttu-id="afdee-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="afdee-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="afdee-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="afdee-135">JSON Representation</span></span>
<span data-ttu-id="afdee-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="afdee-136">Here is a JSON representation of the resource.</span></span>
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





