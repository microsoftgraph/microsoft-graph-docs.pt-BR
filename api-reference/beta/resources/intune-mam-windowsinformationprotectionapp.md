---
title: Tipo de recurso windowsInformationProtectionApp
description: Aplicativo para proteção de informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fb14092fa9f347e551a4871da69d9a3631b96e8c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579174"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="9a137-103">Tipo de recurso windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="9a137-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="9a137-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9a137-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a137-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9a137-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a137-106">Aplicativo para proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="9a137-106">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="9a137-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9a137-107">Properties</span></span>
|<span data-ttu-id="9a137-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a137-108">Property</span></span>|<span data-ttu-id="9a137-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a137-109">Type</span></span>|<span data-ttu-id="9a137-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a137-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a137-111">displayName</span><span class="sxs-lookup"><span data-stu-id="9a137-111">displayName</span></span>|<span data-ttu-id="9a137-112">String</span><span class="sxs-lookup"><span data-stu-id="9a137-112">String</span></span>|<span data-ttu-id="9a137-113">Nome de exibição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9a137-113">App display name.</span></span>|
|<span data-ttu-id="9a137-114">description</span><span class="sxs-lookup"><span data-stu-id="9a137-114">description</span></span>|<span data-ttu-id="9a137-115">String</span><span class="sxs-lookup"><span data-stu-id="9a137-115">String</span></span>|<span data-ttu-id="9a137-116">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9a137-116">The app's description.</span></span>|
|<span data-ttu-id="9a137-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="9a137-117">publisherName</span></span>|<span data-ttu-id="9a137-118">String</span><span class="sxs-lookup"><span data-stu-id="9a137-118">String</span></span>|<span data-ttu-id="9a137-119">O nome do distribuidor</span><span class="sxs-lookup"><span data-stu-id="9a137-119">The publisher name</span></span>|
|<span data-ttu-id="9a137-120">productName</span><span class="sxs-lookup"><span data-stu-id="9a137-120">productName</span></span>|<span data-ttu-id="9a137-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a137-121">String</span></span>|<span data-ttu-id="9a137-122">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="9a137-122">The product name.</span></span>|
|<span data-ttu-id="9a137-123">negado</span><span class="sxs-lookup"><span data-stu-id="9a137-123">denied</span></span>|<span data-ttu-id="9a137-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="9a137-124">Boolean</span></span>|<span data-ttu-id="9a137-125">Se verdadeiro, é negada proteção ou isenção ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9a137-125">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a137-126">Relações</span><span class="sxs-lookup"><span data-stu-id="9a137-126">Relationships</span></span>
<span data-ttu-id="9a137-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9a137-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a137-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9a137-128">JSON Representation</span></span>
<span data-ttu-id="9a137-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9a137-129">Here is a JSON representation of the resource.</span></span>
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





