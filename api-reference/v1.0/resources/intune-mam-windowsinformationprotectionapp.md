---
title: Tipo de recurso windowsInformationProtectionApp
description: Aplicativo para proteção de informações do Windows
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 250542a7ff87b02ee271c0fbb8682f9855cc24ec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833933"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="de998-103">Tipo de recurso windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="de998-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="de998-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="de998-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de998-105">Aplicativo para proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="de998-105">App for Windows information protection</span></span>
## <a name="properties"></a><span data-ttu-id="de998-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="de998-106">Properties</span></span>
|<span data-ttu-id="de998-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de998-107">Property</span></span>|<span data-ttu-id="de998-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="de998-108">Type</span></span>|<span data-ttu-id="de998-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="de998-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de998-110">displayName</span><span class="sxs-lookup"><span data-stu-id="de998-110">displayName</span></span>|<span data-ttu-id="de998-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de998-111">String</span></span>|<span data-ttu-id="de998-112">Nome de exibição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de998-112">App display name.</span></span>|
|<span data-ttu-id="de998-113">descrição</span><span class="sxs-lookup"><span data-stu-id="de998-113">description</span></span>|<span data-ttu-id="de998-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de998-114">String</span></span>|<span data-ttu-id="de998-115">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de998-115">The app's description.</span></span>|
|<span data-ttu-id="de998-116">publisherName</span><span class="sxs-lookup"><span data-stu-id="de998-116">publisherName</span></span>|<span data-ttu-id="de998-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de998-117">String</span></span>|<span data-ttu-id="de998-118">O nome do distribuidor</span><span class="sxs-lookup"><span data-stu-id="de998-118">The publisher name</span></span>|
|<span data-ttu-id="de998-119">productName</span><span class="sxs-lookup"><span data-stu-id="de998-119">productName</span></span>|<span data-ttu-id="de998-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de998-120">String</span></span>|<span data-ttu-id="de998-121">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="de998-121">The product name.</span></span>|
|<span data-ttu-id="de998-122">negado</span><span class="sxs-lookup"><span data-stu-id="de998-122">denied</span></span>|<span data-ttu-id="de998-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="de998-123">Boolean</span></span>|<span data-ttu-id="de998-124">Se verdadeiro, é negada proteção ou isenção ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="de998-124">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de998-125">Relações</span><span class="sxs-lookup"><span data-stu-id="de998-125">Relationships</span></span>
<span data-ttu-id="de998-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="de998-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="de998-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="de998-127">JSON Representation</span></span>
<span data-ttu-id="de998-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="de998-128">Here is a JSON representation of the resource.</span></span>
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



