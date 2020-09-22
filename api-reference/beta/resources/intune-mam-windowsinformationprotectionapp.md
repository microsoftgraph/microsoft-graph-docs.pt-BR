---
title: Tipo de recurso windowsInformationProtectionApp
description: Aplicativo para proteção de informações do Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 59360d948865e184abab7b9749c764a43b2710d9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030056"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="b1868-103">Tipo de recurso windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="b1868-103">windowsInformationProtectionApp resource type</span></span>

<span data-ttu-id="b1868-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1868-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1868-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b1868-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1868-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b1868-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1868-107">Aplicativo para proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="b1868-107">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="b1868-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1868-108">Properties</span></span>
|<span data-ttu-id="b1868-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1868-109">Property</span></span>|<span data-ttu-id="b1868-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1868-110">Type</span></span>|<span data-ttu-id="b1868-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1868-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1868-112">displayName</span><span class="sxs-lookup"><span data-stu-id="b1868-112">displayName</span></span>|<span data-ttu-id="b1868-113">String</span><span class="sxs-lookup"><span data-stu-id="b1868-113">String</span></span>|<span data-ttu-id="b1868-114">Nome de exibição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b1868-114">App display name.</span></span>|
|<span data-ttu-id="b1868-115">description</span><span class="sxs-lookup"><span data-stu-id="b1868-115">description</span></span>|<span data-ttu-id="b1868-116">String</span><span class="sxs-lookup"><span data-stu-id="b1868-116">String</span></span>|<span data-ttu-id="b1868-117">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b1868-117">The app's description.</span></span>|
|<span data-ttu-id="b1868-118">publisherName</span><span class="sxs-lookup"><span data-stu-id="b1868-118">publisherName</span></span>|<span data-ttu-id="b1868-119">String</span><span class="sxs-lookup"><span data-stu-id="b1868-119">String</span></span>|<span data-ttu-id="b1868-120">O nome do distribuidor</span><span class="sxs-lookup"><span data-stu-id="b1868-120">The publisher name</span></span>|
|<span data-ttu-id="b1868-121">productName</span><span class="sxs-lookup"><span data-stu-id="b1868-121">productName</span></span>|<span data-ttu-id="b1868-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1868-122">String</span></span>|<span data-ttu-id="b1868-123">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="b1868-123">The product name.</span></span>|
|<span data-ttu-id="b1868-124">negado</span><span class="sxs-lookup"><span data-stu-id="b1868-124">denied</span></span>|<span data-ttu-id="b1868-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="b1868-125">Boolean</span></span>|<span data-ttu-id="b1868-126">Se verdadeiro, é negada proteção ou isenção ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b1868-126">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1868-127">Relações</span><span class="sxs-lookup"><span data-stu-id="b1868-127">Relationships</span></span>
<span data-ttu-id="b1868-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b1868-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1868-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1868-129">JSON Representation</span></span>
<span data-ttu-id="b1868-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1868-130">Here is a JSON representation of the resource.</span></span>
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






