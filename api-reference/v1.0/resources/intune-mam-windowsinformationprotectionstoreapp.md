---
title: Tipo de recurso windowsInformationProtectionStoreApp
description: Aplicativo de loja para proteção de informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: aaba3e5a34eb4f985d6afe7879159dd3cff456b8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037615"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="08e33-103">Tipo de recurso windowsInformationProtectionStoreApp</span><span class="sxs-lookup"><span data-stu-id="08e33-103">windowsInformationProtectionStoreApp resource type</span></span>

> <span data-ttu-id="08e33-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="08e33-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08e33-105">Aplicativo de loja para proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="08e33-105">Store App for Windows information protection</span></span>


<span data-ttu-id="08e33-106">Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="08e33-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="08e33-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="08e33-107">Properties</span></span>
|<span data-ttu-id="08e33-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08e33-108">Property</span></span>|<span data-ttu-id="08e33-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="08e33-109">Type</span></span>|<span data-ttu-id="08e33-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="08e33-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08e33-111">displayName</span><span class="sxs-lookup"><span data-stu-id="08e33-111">displayName</span></span>|<span data-ttu-id="08e33-112">String</span><span class="sxs-lookup"><span data-stu-id="08e33-112">String</span></span>|<span data-ttu-id="08e33-113">Nome de exibição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="08e33-113">App display name.</span></span> <span data-ttu-id="08e33-114">Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="08e33-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="08e33-115">descrição</span><span class="sxs-lookup"><span data-stu-id="08e33-115">description</span></span>|<span data-ttu-id="08e33-116">String</span><span class="sxs-lookup"><span data-stu-id="08e33-116">String</span></span>|<span data-ttu-id="08e33-117">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="08e33-117">The app's description.</span></span> <span data-ttu-id="08e33-118">Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="08e33-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="08e33-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="08e33-119">publisherName</span></span>|<span data-ttu-id="08e33-120">String</span><span class="sxs-lookup"><span data-stu-id="08e33-120">String</span></span>|<span data-ttu-id="08e33-121">O nome do fornecedor herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="08e33-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="08e33-122">productName</span><span class="sxs-lookup"><span data-stu-id="08e33-122">productName</span></span>|<span data-ttu-id="08e33-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="08e33-123">String</span></span>|<span data-ttu-id="08e33-124">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="08e33-124">The product name.</span></span> <span data-ttu-id="08e33-125">Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="08e33-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="08e33-126">negado</span><span class="sxs-lookup"><span data-stu-id="08e33-126">denied</span></span>|<span data-ttu-id="08e33-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="08e33-127">Boolean</span></span>|<span data-ttu-id="08e33-128">Se verdadeiro, é negada proteção ou isenção ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="08e33-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="08e33-129">Herdado de [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="08e33-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="08e33-130">Relações</span><span class="sxs-lookup"><span data-stu-id="08e33-130">Relationships</span></span>
<span data-ttu-id="08e33-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="08e33-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08e33-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="08e33-132">JSON Representation</span></span>
<span data-ttu-id="08e33-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="08e33-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionStoreApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```



