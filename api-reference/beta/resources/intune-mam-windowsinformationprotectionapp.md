---
title: Tipo de recurso windowsInformationProtectionApp
description: Aplicativo para proteção de informações do Windows
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 45d428ee18e92e76f5a13c568373219f904fd886
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403683"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="e8eb7-103">Tipo de recurso windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="e8eb7-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="e8eb7-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="e8eb7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e8eb7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e8eb7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e8eb7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e8eb7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8eb7-107">Aplicativo para proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="e8eb7-107">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="e8eb7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e8eb7-108">Properties</span></span>
|<span data-ttu-id="e8eb7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8eb7-109">Property</span></span>|<span data-ttu-id="e8eb7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8eb7-110">Type</span></span>|<span data-ttu-id="e8eb7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8eb7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8eb7-112">displayName</span><span class="sxs-lookup"><span data-stu-id="e8eb7-112">displayName</span></span>|<span data-ttu-id="e8eb7-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8eb7-113">String</span></span>|<span data-ttu-id="e8eb7-114">Nome de exibição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e8eb7-114">App display name.</span></span>|
|<span data-ttu-id="e8eb7-115">descrição</span><span class="sxs-lookup"><span data-stu-id="e8eb7-115">description</span></span>|<span data-ttu-id="e8eb7-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8eb7-116">String</span></span>|<span data-ttu-id="e8eb7-117">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e8eb7-117">The app's description.</span></span>|
|<span data-ttu-id="e8eb7-118">publisherName</span><span class="sxs-lookup"><span data-stu-id="e8eb7-118">publisherName</span></span>|<span data-ttu-id="e8eb7-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8eb7-119">String</span></span>|<span data-ttu-id="e8eb7-120">O nome do distribuidor</span><span class="sxs-lookup"><span data-stu-id="e8eb7-120">The publisher name</span></span>|
|<span data-ttu-id="e8eb7-121">productName</span><span class="sxs-lookup"><span data-stu-id="e8eb7-121">productName</span></span>|<span data-ttu-id="e8eb7-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e8eb7-122">String</span></span>|<span data-ttu-id="e8eb7-123">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="e8eb7-123">The product name.</span></span>|
|<span data-ttu-id="e8eb7-124">negado</span><span class="sxs-lookup"><span data-stu-id="e8eb7-124">denied</span></span>|<span data-ttu-id="e8eb7-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="e8eb7-125">Boolean</span></span>|<span data-ttu-id="e8eb7-126">Se verdadeiro, é negada proteção ou isenção ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e8eb7-126">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8eb7-127">Relações</span><span class="sxs-lookup"><span data-stu-id="e8eb7-127">Relationships</span></span>
<span data-ttu-id="e8eb7-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e8eb7-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8eb7-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e8eb7-129">JSON Representation</span></span>
<span data-ttu-id="e8eb7-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e8eb7-130">Here is a JSON representation of the resource.</span></span>
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




