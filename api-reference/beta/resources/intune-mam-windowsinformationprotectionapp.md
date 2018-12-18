---
title: Tipo de recurso windowsInformationProtectionApp
description: Aplicativo para proteção de informações do Windows
author: tfitzmac
ms.openlocfilehash: 6ad47301dc7ec9650026021a2131d34b4d704e70
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334381"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="32fcb-103">Tipo de recurso windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="32fcb-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="32fcb-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="32fcb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32fcb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="32fcb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="32fcb-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="32fcb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="32fcb-107">Aplicativo para proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="32fcb-107">App for Windows information protection</span></span>
## <a name="properties"></a><span data-ttu-id="32fcb-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="32fcb-108">Properties</span></span>
|<span data-ttu-id="32fcb-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32fcb-109">Property</span></span>|<span data-ttu-id="32fcb-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="32fcb-110">Type</span></span>|<span data-ttu-id="32fcb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="32fcb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32fcb-112">displayName</span><span class="sxs-lookup"><span data-stu-id="32fcb-112">displayName</span></span>|<span data-ttu-id="32fcb-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32fcb-113">String</span></span>|<span data-ttu-id="32fcb-114">Nome de exibição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="32fcb-114">App display name.</span></span>|
|<span data-ttu-id="32fcb-115">descrição</span><span class="sxs-lookup"><span data-stu-id="32fcb-115">description</span></span>|<span data-ttu-id="32fcb-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32fcb-116">String</span></span>|<span data-ttu-id="32fcb-117">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="32fcb-117">The app's description.</span></span>|
|<span data-ttu-id="32fcb-118">publisherName</span><span class="sxs-lookup"><span data-stu-id="32fcb-118">publisherName</span></span>|<span data-ttu-id="32fcb-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32fcb-119">String</span></span>|<span data-ttu-id="32fcb-120">O nome do distribuidor</span><span class="sxs-lookup"><span data-stu-id="32fcb-120">The publisher name</span></span>|
|<span data-ttu-id="32fcb-121">productName</span><span class="sxs-lookup"><span data-stu-id="32fcb-121">productName</span></span>|<span data-ttu-id="32fcb-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="32fcb-122">String</span></span>|<span data-ttu-id="32fcb-123">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="32fcb-123">The product name.</span></span>|
|<span data-ttu-id="32fcb-124">negado</span><span class="sxs-lookup"><span data-stu-id="32fcb-124">denied</span></span>|<span data-ttu-id="32fcb-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="32fcb-125">Boolean</span></span>|<span data-ttu-id="32fcb-126">Se verdadeiro, é negada proteção ou isenção ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="32fcb-126">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32fcb-127">Relações</span><span class="sxs-lookup"><span data-stu-id="32fcb-127">Relationships</span></span>
<span data-ttu-id="32fcb-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="32fcb-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="32fcb-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="32fcb-129">JSON Representation</span></span>
<span data-ttu-id="32fcb-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="32fcb-130">Here is a JSON representation of the resource.</span></span>
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





