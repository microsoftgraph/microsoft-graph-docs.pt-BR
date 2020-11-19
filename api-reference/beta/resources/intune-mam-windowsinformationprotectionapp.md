---
title: Tipo de recurso windowsInformationProtectionApp
description: Aplicativo para proteção de informações do Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ada71a184dd0d7f25c774920b6f7d6b3da9fa438
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49297718"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="366b5-103">Tipo de recurso windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="366b5-103">windowsInformationProtectionApp resource type</span></span>

<span data-ttu-id="366b5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="366b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="366b5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="366b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="366b5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="366b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="366b5-107">Aplicativo para proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="366b5-107">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="366b5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="366b5-108">Properties</span></span>
|<span data-ttu-id="366b5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="366b5-109">Property</span></span>|<span data-ttu-id="366b5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="366b5-110">Type</span></span>|<span data-ttu-id="366b5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="366b5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="366b5-112">displayName</span><span class="sxs-lookup"><span data-stu-id="366b5-112">displayName</span></span>|<span data-ttu-id="366b5-113">String</span><span class="sxs-lookup"><span data-stu-id="366b5-113">String</span></span>|<span data-ttu-id="366b5-114">Nome de exibição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="366b5-114">App display name.</span></span>|
|<span data-ttu-id="366b5-115">description</span><span class="sxs-lookup"><span data-stu-id="366b5-115">description</span></span>|<span data-ttu-id="366b5-116">String</span><span class="sxs-lookup"><span data-stu-id="366b5-116">String</span></span>|<span data-ttu-id="366b5-117">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="366b5-117">The app's description.</span></span>|
|<span data-ttu-id="366b5-118">publisherName</span><span class="sxs-lookup"><span data-stu-id="366b5-118">publisherName</span></span>|<span data-ttu-id="366b5-119">String</span><span class="sxs-lookup"><span data-stu-id="366b5-119">String</span></span>|<span data-ttu-id="366b5-120">O nome do distribuidor</span><span class="sxs-lookup"><span data-stu-id="366b5-120">The publisher name</span></span>|
|<span data-ttu-id="366b5-121">productName</span><span class="sxs-lookup"><span data-stu-id="366b5-121">productName</span></span>|<span data-ttu-id="366b5-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="366b5-122">String</span></span>|<span data-ttu-id="366b5-123">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="366b5-123">The product name.</span></span>|
|<span data-ttu-id="366b5-124">negado</span><span class="sxs-lookup"><span data-stu-id="366b5-124">denied</span></span>|<span data-ttu-id="366b5-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="366b5-125">Boolean</span></span>|<span data-ttu-id="366b5-126">Se verdadeiro, é negada proteção ou isenção ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="366b5-126">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="366b5-127">Relações</span><span class="sxs-lookup"><span data-stu-id="366b5-127">Relationships</span></span>
<span data-ttu-id="366b5-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="366b5-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="366b5-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="366b5-129">JSON Representation</span></span>
<span data-ttu-id="366b5-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="366b5-130">Here is a JSON representation of the resource.</span></span>
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




