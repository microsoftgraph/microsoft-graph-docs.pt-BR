---
title: Tipo de recurso windowsInformationProtectionApp
description: Aplicativo para proteção de informações do Windows
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 97e1e866dc71b08064fe46878c25cb5b43c90177
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533333"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="9ba90-103">Tipo de recurso windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="9ba90-103">windowsInformationProtectionApp resource type</span></span>

<span data-ttu-id="9ba90-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ba90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ba90-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9ba90-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ba90-106">Aplicativo para proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="9ba90-106">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="9ba90-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9ba90-107">Properties</span></span>
|<span data-ttu-id="9ba90-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ba90-108">Property</span></span>|<span data-ttu-id="9ba90-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ba90-109">Type</span></span>|<span data-ttu-id="9ba90-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ba90-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ba90-111">displayName</span><span class="sxs-lookup"><span data-stu-id="9ba90-111">displayName</span></span>|<span data-ttu-id="9ba90-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ba90-112">String</span></span>|<span data-ttu-id="9ba90-113">Nome de exibição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9ba90-113">App display name.</span></span>|
|<span data-ttu-id="9ba90-114">description</span><span class="sxs-lookup"><span data-stu-id="9ba90-114">description</span></span>|<span data-ttu-id="9ba90-115">String</span><span class="sxs-lookup"><span data-stu-id="9ba90-115">String</span></span>|<span data-ttu-id="9ba90-116">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9ba90-116">The app's description.</span></span>|
|<span data-ttu-id="9ba90-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="9ba90-117">publisherName</span></span>|<span data-ttu-id="9ba90-118">String</span><span class="sxs-lookup"><span data-stu-id="9ba90-118">String</span></span>|<span data-ttu-id="9ba90-119">O nome do distribuidor</span><span class="sxs-lookup"><span data-stu-id="9ba90-119">The publisher name</span></span>|
|<span data-ttu-id="9ba90-120">productName</span><span class="sxs-lookup"><span data-stu-id="9ba90-120">productName</span></span>|<span data-ttu-id="9ba90-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9ba90-121">String</span></span>|<span data-ttu-id="9ba90-122">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="9ba90-122">The product name.</span></span>|
|<span data-ttu-id="9ba90-123">negado</span><span class="sxs-lookup"><span data-stu-id="9ba90-123">denied</span></span>|<span data-ttu-id="9ba90-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="9ba90-124">Boolean</span></span>|<span data-ttu-id="9ba90-125">Se verdadeiro, é negada proteção ou isenção ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9ba90-125">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ba90-126">Relações</span><span class="sxs-lookup"><span data-stu-id="9ba90-126">Relationships</span></span>
<span data-ttu-id="9ba90-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9ba90-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ba90-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ba90-128">JSON Representation</span></span>
<span data-ttu-id="9ba90-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9ba90-129">Here is a JSON representation of the resource.</span></span>
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




