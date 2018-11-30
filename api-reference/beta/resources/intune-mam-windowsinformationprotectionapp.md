---
title: Tipo de recurso windowsInformationProtectionApp
description: Aplicativo para proteção de informações do Windows
ms.openlocfilehash: 6f5bf2cd42ba2df96f3e9cc2b9b1c1954420c572
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040116"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="99b60-103">Tipo de recurso windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="99b60-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="99b60-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="99b60-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99b60-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="99b60-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="99b60-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="99b60-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99b60-107">Aplicativo para proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="99b60-107">App for Windows information protection</span></span>
## <a name="properties"></a><span data-ttu-id="99b60-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99b60-108">Properties</span></span>
|<span data-ttu-id="99b60-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99b60-109">Property</span></span>|<span data-ttu-id="99b60-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="99b60-110">Type</span></span>|<span data-ttu-id="99b60-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="99b60-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99b60-112">displayName</span><span class="sxs-lookup"><span data-stu-id="99b60-112">displayName</span></span>|<span data-ttu-id="99b60-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99b60-113">String</span></span>|<span data-ttu-id="99b60-114">Nome de exibição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="99b60-114">App display name.</span></span>|
|<span data-ttu-id="99b60-115">descrição</span><span class="sxs-lookup"><span data-stu-id="99b60-115">description</span></span>|<span data-ttu-id="99b60-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99b60-116">String</span></span>|<span data-ttu-id="99b60-117">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="99b60-117">The app's description.</span></span>|
|<span data-ttu-id="99b60-118">publisherName</span><span class="sxs-lookup"><span data-stu-id="99b60-118">publisherName</span></span>|<span data-ttu-id="99b60-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99b60-119">String</span></span>|<span data-ttu-id="99b60-120">O nome do distribuidor</span><span class="sxs-lookup"><span data-stu-id="99b60-120">The publisher name</span></span>|
|<span data-ttu-id="99b60-121">productName</span><span class="sxs-lookup"><span data-stu-id="99b60-121">productName</span></span>|<span data-ttu-id="99b60-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99b60-122">String</span></span>|<span data-ttu-id="99b60-123">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="99b60-123">The product name.</span></span>|
|<span data-ttu-id="99b60-124">negado</span><span class="sxs-lookup"><span data-stu-id="99b60-124">denied</span></span>|<span data-ttu-id="99b60-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="99b60-125">Boolean</span></span>|<span data-ttu-id="99b60-126">Se verdadeiro, é negada proteção ou isenção ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="99b60-126">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99b60-127">Relações</span><span class="sxs-lookup"><span data-stu-id="99b60-127">Relationships</span></span>
<span data-ttu-id="99b60-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="99b60-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="99b60-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99b60-129">JSON Representation</span></span>
<span data-ttu-id="99b60-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="99b60-130">Here is a JSON representation of the resource.</span></span>
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





