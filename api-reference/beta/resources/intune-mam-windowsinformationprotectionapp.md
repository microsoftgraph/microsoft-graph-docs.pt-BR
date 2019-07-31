---
title: Tipo de recurso windowsInformationProtectionApp
description: Aplicativo para proteção de informações do Windows
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 61ada685166fbe3ca7ef02fa8f87e5383666e9ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967895"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="3efa3-103">Tipo de recurso windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="3efa3-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="3efa3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3efa3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3efa3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3efa3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3efa3-106">Aplicativo para proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="3efa3-106">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="3efa3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3efa3-107">Properties</span></span>
|<span data-ttu-id="3efa3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3efa3-108">Property</span></span>|<span data-ttu-id="3efa3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3efa3-109">Type</span></span>|<span data-ttu-id="3efa3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3efa3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3efa3-111">displayName</span><span class="sxs-lookup"><span data-stu-id="3efa3-111">displayName</span></span>|<span data-ttu-id="3efa3-112">String</span><span class="sxs-lookup"><span data-stu-id="3efa3-112">String</span></span>|<span data-ttu-id="3efa3-113">Nome de exibição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3efa3-113">App display name.</span></span>|
|<span data-ttu-id="3efa3-114">descrição</span><span class="sxs-lookup"><span data-stu-id="3efa3-114">description</span></span>|<span data-ttu-id="3efa3-115">String</span><span class="sxs-lookup"><span data-stu-id="3efa3-115">String</span></span>|<span data-ttu-id="3efa3-116">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3efa3-116">The app's description.</span></span>|
|<span data-ttu-id="3efa3-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="3efa3-117">publisherName</span></span>|<span data-ttu-id="3efa3-118">String</span><span class="sxs-lookup"><span data-stu-id="3efa3-118">String</span></span>|<span data-ttu-id="3efa3-119">O nome do distribuidor</span><span class="sxs-lookup"><span data-stu-id="3efa3-119">The publisher name</span></span>|
|<span data-ttu-id="3efa3-120">productName</span><span class="sxs-lookup"><span data-stu-id="3efa3-120">productName</span></span>|<span data-ttu-id="3efa3-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3efa3-121">String</span></span>|<span data-ttu-id="3efa3-122">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="3efa3-122">The product name.</span></span>|
|<span data-ttu-id="3efa3-123">negado</span><span class="sxs-lookup"><span data-stu-id="3efa3-123">denied</span></span>|<span data-ttu-id="3efa3-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="3efa3-124">Boolean</span></span>|<span data-ttu-id="3efa3-125">Se verdadeiro, é negada proteção ou isenção ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3efa3-125">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3efa3-126">Relações</span><span class="sxs-lookup"><span data-stu-id="3efa3-126">Relationships</span></span>
<span data-ttu-id="3efa3-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3efa3-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3efa3-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3efa3-128">JSON Representation</span></span>
<span data-ttu-id="3efa3-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3efa3-129">Here is a JSON representation of the resource.</span></span>
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





