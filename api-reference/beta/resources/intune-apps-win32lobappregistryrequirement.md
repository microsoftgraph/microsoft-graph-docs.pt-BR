---
title: tipo de recurso win32LobAppRegistryRequirement
description: Contém as propriedades do registro para detectar um aplicativo Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 860bb42b4ed175310e8cd8491f242b2cb87cafd1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49280715"
---
# <a name="win32lobappregistryrequirement-resource-type"></a><span data-ttu-id="fbb52-103">tipo de recurso win32LobAppRegistryRequirement</span><span class="sxs-lookup"><span data-stu-id="fbb52-103">win32LobAppRegistryRequirement resource type</span></span>

<span data-ttu-id="fbb52-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbb52-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fbb52-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="fbb52-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbb52-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fbb52-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbb52-107">Contém as propriedades do registro para detectar um aplicativo Win32</span><span class="sxs-lookup"><span data-stu-id="fbb52-107">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="fbb52-108">Herda de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="fbb52-108">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fbb52-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fbb52-109">Properties</span></span>
|<span data-ttu-id="fbb52-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbb52-110">Property</span></span>|<span data-ttu-id="fbb52-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbb52-111">Type</span></span>|<span data-ttu-id="fbb52-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbb52-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbb52-113">operator</span><span class="sxs-lookup"><span data-stu-id="fbb52-113">operator</span></span>|[<span data-ttu-id="fbb52-114">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="fbb52-114">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="fbb52-115">O operador para detecção herdada de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span><span class="sxs-lookup"><span data-stu-id="fbb52-115">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="fbb52-116">Os valores possíveis são: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="fbb52-116">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="fbb52-117">detecçaovalue</span><span class="sxs-lookup"><span data-stu-id="fbb52-117">detectionValue</span></span>|<span data-ttu-id="fbb52-118">String</span><span class="sxs-lookup"><span data-stu-id="fbb52-118">String</span></span>|<span data-ttu-id="fbb52-119">O valor de detecção herdado de [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="fbb52-119">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="fbb52-120">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="fbb52-120">check32BitOn64System</span></span>|<span data-ttu-id="fbb52-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="fbb52-121">Boolean</span></span>|<span data-ttu-id="fbb52-122">Um valor que indica se este caminho de registro é para verificar o aplicativo de 32 bits no sistema de 64 bits</span><span class="sxs-lookup"><span data-stu-id="fbb52-122">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="fbb52-123">Caminho-chave</span><span class="sxs-lookup"><span data-stu-id="fbb52-123">keyPath</span></span>|<span data-ttu-id="fbb52-124">String</span><span class="sxs-lookup"><span data-stu-id="fbb52-124">String</span></span>|<span data-ttu-id="fbb52-125">O caminho da chave do registro para detectar o aplicativo de LoB (linha de negócios) do Win32</span><span class="sxs-lookup"><span data-stu-id="fbb52-125">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="fbb52-126">valueName</span><span class="sxs-lookup"><span data-stu-id="fbb52-126">valueName</span></span>|<span data-ttu-id="fbb52-127">String</span><span class="sxs-lookup"><span data-stu-id="fbb52-127">String</span></span>|<span data-ttu-id="fbb52-128">O nome do valor do registro</span><span class="sxs-lookup"><span data-stu-id="fbb52-128">The registry value name</span></span>|
|<span data-ttu-id="fbb52-129">Detecção</span><span class="sxs-lookup"><span data-stu-id="fbb52-129">detectionType</span></span>|[<span data-ttu-id="fbb52-130">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="fbb52-130">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="fbb52-131">O tipo de detecção de dados do registro.</span><span class="sxs-lookup"><span data-stu-id="fbb52-131">The registry data detection type.</span></span> <span data-ttu-id="fbb52-132">Os possíveis valores são: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="fbb52-132">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbb52-133">Relações</span><span class="sxs-lookup"><span data-stu-id="fbb52-133">Relationships</span></span>
<span data-ttu-id="fbb52-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fbb52-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fbb52-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fbb52-135">JSON Representation</span></span>
<span data-ttu-id="fbb52-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fbb52-136">Here is a JSON representation of the resource.</span></span>
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




