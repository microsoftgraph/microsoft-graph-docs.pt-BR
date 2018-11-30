---
title: Tipo de recurso windowsInformationProtectionApp
description: Aplicativo para proteção de informações do Windows
ms.openlocfilehash: 0ea48e087d4a8450ee47b2239b7c67f3b050da85
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004101"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="6cfd9-103">Tipo de recurso windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="6cfd9-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="6cfd9-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6cfd9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6cfd9-105">Aplicativo para proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="6cfd9-105">App for Windows information protection</span></span>
## <a name="properties"></a><span data-ttu-id="6cfd9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6cfd9-106">Properties</span></span>
|<span data-ttu-id="6cfd9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6cfd9-107">Property</span></span>|<span data-ttu-id="6cfd9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6cfd9-108">Type</span></span>|<span data-ttu-id="6cfd9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cfd9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cfd9-110">displayName</span><span class="sxs-lookup"><span data-stu-id="6cfd9-110">displayName</span></span>|<span data-ttu-id="6cfd9-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6cfd9-111">String</span></span>|<span data-ttu-id="6cfd9-112">Nome de exibição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cfd9-112">App display name.</span></span>|
|<span data-ttu-id="6cfd9-113">descrição</span><span class="sxs-lookup"><span data-stu-id="6cfd9-113">description</span></span>|<span data-ttu-id="6cfd9-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6cfd9-114">String</span></span>|<span data-ttu-id="6cfd9-115">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cfd9-115">The app's description.</span></span>|
|<span data-ttu-id="6cfd9-116">publisherName</span><span class="sxs-lookup"><span data-stu-id="6cfd9-116">publisherName</span></span>|<span data-ttu-id="6cfd9-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6cfd9-117">String</span></span>|<span data-ttu-id="6cfd9-118">O nome do distribuidor</span><span class="sxs-lookup"><span data-stu-id="6cfd9-118">The publisher name</span></span>|
|<span data-ttu-id="6cfd9-119">productName</span><span class="sxs-lookup"><span data-stu-id="6cfd9-119">productName</span></span>|<span data-ttu-id="6cfd9-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6cfd9-120">String</span></span>|<span data-ttu-id="6cfd9-121">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="6cfd9-121">The product name.</span></span>|
|<span data-ttu-id="6cfd9-122">negado</span><span class="sxs-lookup"><span data-stu-id="6cfd9-122">denied</span></span>|<span data-ttu-id="6cfd9-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="6cfd9-123">Boolean</span></span>|<span data-ttu-id="6cfd9-124">Se verdadeiro, é negada proteção ou isenção ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6cfd9-124">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6cfd9-125">Relações</span><span class="sxs-lookup"><span data-stu-id="6cfd9-125">Relationships</span></span>
<span data-ttu-id="6cfd9-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6cfd9-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6cfd9-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6cfd9-127">JSON Representation</span></span>
<span data-ttu-id="6cfd9-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6cfd9-128">Here is a JSON representation of the resource.</span></span>
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



