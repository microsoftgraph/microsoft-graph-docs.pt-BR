---
title: Tipo de recurso windowsInformationProtectionDesktopApp
description: Aplicativo da área de trabalho para a proteção de informações do Windows
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d570420512e9da31fcd95efd2df2c2a3e1da83c9
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367305"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="2fd91-103">Tipo de recurso windowsInformationProtectionDesktopApp</span><span class="sxs-lookup"><span data-stu-id="2fd91-103">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="2fd91-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2fd91-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fd91-105">Aplicativo da área de trabalho para a proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="2fd91-105">Desktop App for Windows information protection</span></span>


<span data-ttu-id="2fd91-106">Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="2fd91-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2fd91-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2fd91-107">Properties</span></span>
|<span data-ttu-id="2fd91-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2fd91-108">Property</span></span>|<span data-ttu-id="2fd91-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fd91-109">Type</span></span>|<span data-ttu-id="2fd91-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fd91-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fd91-111">displayName</span><span class="sxs-lookup"><span data-stu-id="2fd91-111">displayName</span></span>|<span data-ttu-id="2fd91-112">String</span><span class="sxs-lookup"><span data-stu-id="2fd91-112">String</span></span>|<span data-ttu-id="2fd91-113">Nome de exibição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2fd91-113">App display name.</span></span> <span data-ttu-id="2fd91-114">Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="2fd91-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="2fd91-115">descrição</span><span class="sxs-lookup"><span data-stu-id="2fd91-115">description</span></span>|<span data-ttu-id="2fd91-116">String</span><span class="sxs-lookup"><span data-stu-id="2fd91-116">String</span></span>|<span data-ttu-id="2fd91-117">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2fd91-117">The app's description.</span></span> <span data-ttu-id="2fd91-118">Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="2fd91-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="2fd91-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="2fd91-119">publisherName</span></span>|<span data-ttu-id="2fd91-120">String</span><span class="sxs-lookup"><span data-stu-id="2fd91-120">String</span></span>|<span data-ttu-id="2fd91-121">O nome do fornecedor herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="2fd91-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="2fd91-122">productName</span><span class="sxs-lookup"><span data-stu-id="2fd91-122">productName</span></span>|<span data-ttu-id="2fd91-123">String</span><span class="sxs-lookup"><span data-stu-id="2fd91-123">String</span></span>|<span data-ttu-id="2fd91-124">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="2fd91-124">The product name.</span></span> <span data-ttu-id="2fd91-125">Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="2fd91-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="2fd91-126">negado</span><span class="sxs-lookup"><span data-stu-id="2fd91-126">denied</span></span>|<span data-ttu-id="2fd91-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="2fd91-127">Boolean</span></span>|<span data-ttu-id="2fd91-128">Se verdadeiro, é negada proteção ou isenção ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2fd91-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="2fd91-129">Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="2fd91-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="2fd91-130">binaryName</span><span class="sxs-lookup"><span data-stu-id="2fd91-130">binaryName</span></span>|<span data-ttu-id="2fd91-131">String</span><span class="sxs-lookup"><span data-stu-id="2fd91-131">String</span></span>|<span data-ttu-id="2fd91-132">O nome binário.</span><span class="sxs-lookup"><span data-stu-id="2fd91-132">The binary name.</span></span>|
|<span data-ttu-id="2fd91-133">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="2fd91-133">binaryVersionLow</span></span>|<span data-ttu-id="2fd91-134">String</span><span class="sxs-lookup"><span data-stu-id="2fd91-134">String</span></span>|<span data-ttu-id="2fd91-135">A versão binária inferior.</span><span class="sxs-lookup"><span data-stu-id="2fd91-135">The lower binary version.</span></span>|
|<span data-ttu-id="2fd91-136">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="2fd91-136">binaryVersionHigh</span></span>|<span data-ttu-id="2fd91-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2fd91-137">String</span></span>|<span data-ttu-id="2fd91-138">A versão binária superior.</span><span class="sxs-lookup"><span data-stu-id="2fd91-138">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fd91-139">Relações</span><span class="sxs-lookup"><span data-stu-id="2fd91-139">Relationships</span></span>
<span data-ttu-id="2fd91-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2fd91-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2fd91-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2fd91-141">JSON Representation</span></span>
<span data-ttu-id="2fd91-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2fd91-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDesktopApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true,
  "binaryName": "String",
  "binaryVersionLow": "String",
  "binaryVersionHigh": "String"
}
```




