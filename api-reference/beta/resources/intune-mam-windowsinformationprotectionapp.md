---
title: Tipo de recurso windowsInformationProtectionApp
description: Aplicativo para proteção de informações do Windows
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1e7cd7225783edd3e2e86d4d60ea2705568245d5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524270"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="a283d-103">Tipo de recurso windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="a283d-103">windowsInformationProtectionApp resource type</span></span>

<span data-ttu-id="a283d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a283d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a283d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a283d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a283d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a283d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a283d-107">Aplicativo para proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="a283d-107">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="a283d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a283d-108">Properties</span></span>
|<span data-ttu-id="a283d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a283d-109">Property</span></span>|<span data-ttu-id="a283d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a283d-110">Type</span></span>|<span data-ttu-id="a283d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a283d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a283d-112">displayName</span><span class="sxs-lookup"><span data-stu-id="a283d-112">displayName</span></span>|<span data-ttu-id="a283d-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a283d-113">String</span></span>|<span data-ttu-id="a283d-114">Nome de exibição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a283d-114">App display name.</span></span>|
|<span data-ttu-id="a283d-115">description</span><span class="sxs-lookup"><span data-stu-id="a283d-115">description</span></span>|<span data-ttu-id="a283d-116">String</span><span class="sxs-lookup"><span data-stu-id="a283d-116">String</span></span>|<span data-ttu-id="a283d-117">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a283d-117">The app's description.</span></span>|
|<span data-ttu-id="a283d-118">publisherName</span><span class="sxs-lookup"><span data-stu-id="a283d-118">publisherName</span></span>|<span data-ttu-id="a283d-119">String</span><span class="sxs-lookup"><span data-stu-id="a283d-119">String</span></span>|<span data-ttu-id="a283d-120">O nome do distribuidor</span><span class="sxs-lookup"><span data-stu-id="a283d-120">The publisher name</span></span>|
|<span data-ttu-id="a283d-121">productName</span><span class="sxs-lookup"><span data-stu-id="a283d-121">productName</span></span>|<span data-ttu-id="a283d-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a283d-122">String</span></span>|<span data-ttu-id="a283d-123">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="a283d-123">The product name.</span></span>|
|<span data-ttu-id="a283d-124">negado</span><span class="sxs-lookup"><span data-stu-id="a283d-124">denied</span></span>|<span data-ttu-id="a283d-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="a283d-125">Boolean</span></span>|<span data-ttu-id="a283d-126">Se verdadeiro, é negada proteção ou isenção ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a283d-126">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a283d-127">Relações</span><span class="sxs-lookup"><span data-stu-id="a283d-127">Relationships</span></span>
<span data-ttu-id="a283d-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a283d-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a283d-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a283d-129">JSON Representation</span></span>
<span data-ttu-id="a283d-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a283d-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```



