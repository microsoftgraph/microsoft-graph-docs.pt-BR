---
title: Tipo de recurso windowsInformationProtectionApp
description: Aplicativo para proteção de informações do Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: be46da02dae93199ae18306bba361a5036e21e3e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079246"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="ac6f4-103">Tipo de recurso windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="ac6f4-103">windowsInformationProtectionApp resource type</span></span>

<span data-ttu-id="ac6f4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac6f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ac6f4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ac6f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac6f4-106">Aplicativo para proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="ac6f4-106">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="ac6f4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac6f4-107">Properties</span></span>
|<span data-ttu-id="ac6f4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac6f4-108">Property</span></span>|<span data-ttu-id="ac6f4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac6f4-109">Type</span></span>|<span data-ttu-id="ac6f4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac6f4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac6f4-111">displayName</span><span class="sxs-lookup"><span data-stu-id="ac6f4-111">displayName</span></span>|<span data-ttu-id="ac6f4-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac6f4-112">String</span></span>|<span data-ttu-id="ac6f4-113">Nome de exibição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ac6f4-113">App display name.</span></span>|
|<span data-ttu-id="ac6f4-114">description</span><span class="sxs-lookup"><span data-stu-id="ac6f4-114">description</span></span>|<span data-ttu-id="ac6f4-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac6f4-115">String</span></span>|<span data-ttu-id="ac6f4-116">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ac6f4-116">The app's description.</span></span>|
|<span data-ttu-id="ac6f4-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="ac6f4-117">publisherName</span></span>|<span data-ttu-id="ac6f4-118">String</span><span class="sxs-lookup"><span data-stu-id="ac6f4-118">String</span></span>|<span data-ttu-id="ac6f4-119">O nome do distribuidor</span><span class="sxs-lookup"><span data-stu-id="ac6f4-119">The publisher name</span></span>|
|<span data-ttu-id="ac6f4-120">productName</span><span class="sxs-lookup"><span data-stu-id="ac6f4-120">productName</span></span>|<span data-ttu-id="ac6f4-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac6f4-121">String</span></span>|<span data-ttu-id="ac6f4-122">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="ac6f4-122">The product name.</span></span>|
|<span data-ttu-id="ac6f4-123">negado</span><span class="sxs-lookup"><span data-stu-id="ac6f4-123">denied</span></span>|<span data-ttu-id="ac6f4-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac6f4-124">Boolean</span></span>|<span data-ttu-id="ac6f4-125">Se verdadeiro, é negada proteção ou isenção ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ac6f4-125">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac6f4-126">Relações</span><span class="sxs-lookup"><span data-stu-id="ac6f4-126">Relationships</span></span>
<span data-ttu-id="ac6f4-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ac6f4-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac6f4-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac6f4-128">JSON Representation</span></span>
<span data-ttu-id="ac6f4-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ac6f4-129">Here is a JSON representation of the resource.</span></span>
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









