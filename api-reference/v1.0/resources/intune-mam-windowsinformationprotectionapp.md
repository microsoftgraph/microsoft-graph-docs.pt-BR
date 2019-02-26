---
title: Tipo de recurso windowsInformationProtectionApp
description: Aplicativo para proteção de informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 00d329baea829fa8fb7664895382a377f53461ab
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257033"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="46ccc-103">Tipo de recurso windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="46ccc-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="46ccc-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="46ccc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46ccc-105">Aplicativo para proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="46ccc-105">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="46ccc-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="46ccc-106">Properties</span></span>
|<span data-ttu-id="46ccc-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="46ccc-107">Property</span></span>|<span data-ttu-id="46ccc-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="46ccc-108">Type</span></span>|<span data-ttu-id="46ccc-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="46ccc-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46ccc-110">displayName</span><span class="sxs-lookup"><span data-stu-id="46ccc-110">displayName</span></span>|<span data-ttu-id="46ccc-111">String</span><span class="sxs-lookup"><span data-stu-id="46ccc-111">String</span></span>|<span data-ttu-id="46ccc-112">Nome de exibição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="46ccc-112">App display name.</span></span>|
|<span data-ttu-id="46ccc-113">descrição</span><span class="sxs-lookup"><span data-stu-id="46ccc-113">description</span></span>|<span data-ttu-id="46ccc-114">String</span><span class="sxs-lookup"><span data-stu-id="46ccc-114">String</span></span>|<span data-ttu-id="46ccc-115">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="46ccc-115">The app's description.</span></span>|
|<span data-ttu-id="46ccc-116">publisherName</span><span class="sxs-lookup"><span data-stu-id="46ccc-116">publisherName</span></span>|<span data-ttu-id="46ccc-117">String</span><span class="sxs-lookup"><span data-stu-id="46ccc-117">String</span></span>|<span data-ttu-id="46ccc-118">O nome do distribuidor</span><span class="sxs-lookup"><span data-stu-id="46ccc-118">The publisher name</span></span>|
|<span data-ttu-id="46ccc-119">productName</span><span class="sxs-lookup"><span data-stu-id="46ccc-119">productName</span></span>|<span data-ttu-id="46ccc-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="46ccc-120">String</span></span>|<span data-ttu-id="46ccc-121">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="46ccc-121">The product name.</span></span>|
|<span data-ttu-id="46ccc-122">negado</span><span class="sxs-lookup"><span data-stu-id="46ccc-122">denied</span></span>|<span data-ttu-id="46ccc-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="46ccc-123">Boolean</span></span>|<span data-ttu-id="46ccc-124">Se verdadeiro, é negada proteção ou isenção ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="46ccc-124">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="46ccc-125">Relações</span><span class="sxs-lookup"><span data-stu-id="46ccc-125">Relationships</span></span>
<span data-ttu-id="46ccc-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="46ccc-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="46ccc-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="46ccc-127">JSON Representation</span></span>
<span data-ttu-id="46ccc-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="46ccc-128">Here is a JSON representation of the resource.</span></span>
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



