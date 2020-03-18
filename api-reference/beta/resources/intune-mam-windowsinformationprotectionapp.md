---
title: Tipo de recurso windowsInformationProtectionApp
description: Aplicativo para proteção de informações do Windows
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fbaa627cd8665678de148f8338a8570f57a2cb01
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42780966"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="148ea-103">Tipo de recurso windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="148ea-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="148ea-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="148ea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="148ea-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="148ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="148ea-106">Aplicativo para proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="148ea-106">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="148ea-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="148ea-107">Properties</span></span>
|<span data-ttu-id="148ea-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="148ea-108">Property</span></span>|<span data-ttu-id="148ea-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="148ea-109">Type</span></span>|<span data-ttu-id="148ea-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="148ea-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="148ea-111">displayName</span><span class="sxs-lookup"><span data-stu-id="148ea-111">displayName</span></span>|<span data-ttu-id="148ea-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="148ea-112">String</span></span>|<span data-ttu-id="148ea-113">Nome de exibição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="148ea-113">App display name.</span></span>|
|<span data-ttu-id="148ea-114">description</span><span class="sxs-lookup"><span data-stu-id="148ea-114">description</span></span>|<span data-ttu-id="148ea-115">String</span><span class="sxs-lookup"><span data-stu-id="148ea-115">String</span></span>|<span data-ttu-id="148ea-116">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="148ea-116">The app's description.</span></span>|
|<span data-ttu-id="148ea-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="148ea-117">publisherName</span></span>|<span data-ttu-id="148ea-118">String</span><span class="sxs-lookup"><span data-stu-id="148ea-118">String</span></span>|<span data-ttu-id="148ea-119">O nome do distribuidor</span><span class="sxs-lookup"><span data-stu-id="148ea-119">The publisher name</span></span>|
|<span data-ttu-id="148ea-120">productName</span><span class="sxs-lookup"><span data-stu-id="148ea-120">productName</span></span>|<span data-ttu-id="148ea-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="148ea-121">String</span></span>|<span data-ttu-id="148ea-122">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="148ea-122">The product name.</span></span>|
|<span data-ttu-id="148ea-123">negado</span><span class="sxs-lookup"><span data-stu-id="148ea-123">denied</span></span>|<span data-ttu-id="148ea-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="148ea-124">Boolean</span></span>|<span data-ttu-id="148ea-125">Se verdadeiro, é negada proteção ou isenção ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="148ea-125">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="148ea-126">Relações</span><span class="sxs-lookup"><span data-stu-id="148ea-126">Relationships</span></span>
<span data-ttu-id="148ea-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="148ea-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="148ea-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="148ea-128">JSON Representation</span></span>
<span data-ttu-id="148ea-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="148ea-129">Here is a JSON representation of the resource.</span></span>
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



