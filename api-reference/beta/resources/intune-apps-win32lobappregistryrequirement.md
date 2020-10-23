---
title: tipo de recurso win32LobAppRegistryRequirement
description: Contém as propriedades do registro para detectar um aplicativo Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 175896a3b086821e4c36a26b5644d08e503d019d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706216"
---
# <a name="win32lobappregistryrequirement-resource-type"></a><span data-ttu-id="170b9-103">tipo de recurso win32LobAppRegistryRequirement</span><span class="sxs-lookup"><span data-stu-id="170b9-103">win32LobAppRegistryRequirement resource type</span></span>

<span data-ttu-id="170b9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="170b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="170b9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="170b9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="170b9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="170b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="170b9-107">Contém as propriedades do registro para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="170b9-107">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="170b9-108">Herda de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="170b9-108">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="170b9-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="170b9-109">Properties</span></span>
|<span data-ttu-id="170b9-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="170b9-110">Property</span></span>|<span data-ttu-id="170b9-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="170b9-111">Type</span></span>|<span data-ttu-id="170b9-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="170b9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="170b9-113">operator</span><span class="sxs-lookup"><span data-stu-id="170b9-113">operator</span></span>|[<span data-ttu-id="170b9-114">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="170b9-114">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="170b9-115">O operador para detecção herdada de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span><span class="sxs-lookup"><span data-stu-id="170b9-115">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="170b9-116">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="170b9-116">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="170b9-117">detecçaovalue</span><span class="sxs-lookup"><span data-stu-id="170b9-117">detectionValue</span></span>|<span data-ttu-id="170b9-118">String</span><span class="sxs-lookup"><span data-stu-id="170b9-118">String</span></span>|<span data-ttu-id="170b9-119">O valor de detecção herdado de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="170b9-119">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="170b9-120">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="170b9-120">check32BitOn64System</span></span>|<span data-ttu-id="170b9-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="170b9-121">Boolean</span></span>|<span data-ttu-id="170b9-122">Um valor que indica se este caminho de registro é para verificar o aplicativo de 32 bits no sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="170b9-122">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="170b9-123">Caminho-chave</span><span class="sxs-lookup"><span data-stu-id="170b9-123">keyPath</span></span>|<span data-ttu-id="170b9-124">String</span><span class="sxs-lookup"><span data-stu-id="170b9-124">String</span></span>|<span data-ttu-id="170b9-125">O caminho da chave do registro para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="170b9-125">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="170b9-126">valueName</span><span class="sxs-lookup"><span data-stu-id="170b9-126">valueName</span></span>|<span data-ttu-id="170b9-127">String</span><span class="sxs-lookup"><span data-stu-id="170b9-127">String</span></span>|<span data-ttu-id="170b9-128">O nome do valor do registro</span><span class="sxs-lookup"><span data-stu-id="170b9-128">The registry value name</span></span>|
|<span data-ttu-id="170b9-129">Detecção</span><span class="sxs-lookup"><span data-stu-id="170b9-129">detectionType</span></span>|[<span data-ttu-id="170b9-130">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="170b9-130">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="170b9-131">O tipo de detecção de dados do registro.</span><span class="sxs-lookup"><span data-stu-id="170b9-131">The registry data detection type.</span></span> <span data-ttu-id="170b9-132">Os possíveis valores são: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="170b9-132">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="170b9-133">Relações</span><span class="sxs-lookup"><span data-stu-id="170b9-133">Relationships</span></span>
<span data-ttu-id="170b9-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="170b9-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="170b9-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="170b9-135">JSON Representation</span></span>
<span data-ttu-id="170b9-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="170b9-136">Here is a JSON representation of the resource.</span></span>
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





