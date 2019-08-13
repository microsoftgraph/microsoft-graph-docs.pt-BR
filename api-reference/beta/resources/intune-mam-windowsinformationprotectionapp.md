---
title: Tipo de recurso windowsInformationProtectionApp
description: Aplicativo para proteção de informações do Windows
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 08a1ed7d56c41eee69ee907a9efd91c12fad9b4e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373256"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="c99b9-103">Tipo de recurso windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="c99b9-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="c99b9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c99b9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c99b9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c99b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c99b9-106">Aplicativo para proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="c99b9-106">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="c99b9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c99b9-107">Properties</span></span>
|<span data-ttu-id="c99b9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c99b9-108">Property</span></span>|<span data-ttu-id="c99b9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c99b9-109">Type</span></span>|<span data-ttu-id="c99b9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c99b9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c99b9-111">displayName</span><span class="sxs-lookup"><span data-stu-id="c99b9-111">displayName</span></span>|<span data-ttu-id="c99b9-112">String</span><span class="sxs-lookup"><span data-stu-id="c99b9-112">String</span></span>|<span data-ttu-id="c99b9-113">Nome de exibição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c99b9-113">App display name.</span></span>|
|<span data-ttu-id="c99b9-114">descrição</span><span class="sxs-lookup"><span data-stu-id="c99b9-114">description</span></span>|<span data-ttu-id="c99b9-115">String</span><span class="sxs-lookup"><span data-stu-id="c99b9-115">String</span></span>|<span data-ttu-id="c99b9-116">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c99b9-116">The app's description.</span></span>|
|<span data-ttu-id="c99b9-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="c99b9-117">publisherName</span></span>|<span data-ttu-id="c99b9-118">String</span><span class="sxs-lookup"><span data-stu-id="c99b9-118">String</span></span>|<span data-ttu-id="c99b9-119">O nome do distribuidor</span><span class="sxs-lookup"><span data-stu-id="c99b9-119">The publisher name</span></span>|
|<span data-ttu-id="c99b9-120">productName</span><span class="sxs-lookup"><span data-stu-id="c99b9-120">productName</span></span>|<span data-ttu-id="c99b9-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c99b9-121">String</span></span>|<span data-ttu-id="c99b9-122">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="c99b9-122">The product name.</span></span>|
|<span data-ttu-id="c99b9-123">negado</span><span class="sxs-lookup"><span data-stu-id="c99b9-123">denied</span></span>|<span data-ttu-id="c99b9-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="c99b9-124">Boolean</span></span>|<span data-ttu-id="c99b9-125">Se verdadeiro, é negada proteção ou isenção ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c99b9-125">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c99b9-126">Relações</span><span class="sxs-lookup"><span data-stu-id="c99b9-126">Relationships</span></span>
<span data-ttu-id="c99b9-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c99b9-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c99b9-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c99b9-128">JSON Representation</span></span>
<span data-ttu-id="c99b9-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c99b9-129">Here is a JSON representation of the resource.</span></span>
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



