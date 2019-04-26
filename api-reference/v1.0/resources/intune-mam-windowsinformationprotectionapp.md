---
title: Tipo de recurso windowsInformationProtectionApp
description: Aplicativo para proteção de informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 00d329baea829fa8fb7664895382a377f53461ab
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561199"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="31777-103">Tipo de recurso windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="31777-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="31777-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="31777-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31777-105">Aplicativo para proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="31777-105">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="31777-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="31777-106">Properties</span></span>
|<span data-ttu-id="31777-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31777-107">Property</span></span>|<span data-ttu-id="31777-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="31777-108">Type</span></span>|<span data-ttu-id="31777-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="31777-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31777-110">displayName</span><span class="sxs-lookup"><span data-stu-id="31777-110">displayName</span></span>|<span data-ttu-id="31777-111">String</span><span class="sxs-lookup"><span data-stu-id="31777-111">String</span></span>|<span data-ttu-id="31777-112">Nome de exibição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="31777-112">App display name.</span></span>|
|<span data-ttu-id="31777-113">description</span><span class="sxs-lookup"><span data-stu-id="31777-113">description</span></span>|<span data-ttu-id="31777-114">String</span><span class="sxs-lookup"><span data-stu-id="31777-114">String</span></span>|<span data-ttu-id="31777-115">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="31777-115">The app's description.</span></span>|
|<span data-ttu-id="31777-116">publisherName</span><span class="sxs-lookup"><span data-stu-id="31777-116">publisherName</span></span>|<span data-ttu-id="31777-117">String</span><span class="sxs-lookup"><span data-stu-id="31777-117">String</span></span>|<span data-ttu-id="31777-118">O nome do distribuidor</span><span class="sxs-lookup"><span data-stu-id="31777-118">The publisher name</span></span>|
|<span data-ttu-id="31777-119">productName</span><span class="sxs-lookup"><span data-stu-id="31777-119">productName</span></span>|<span data-ttu-id="31777-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="31777-120">String</span></span>|<span data-ttu-id="31777-121">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="31777-121">The product name.</span></span>|
|<span data-ttu-id="31777-122">negado</span><span class="sxs-lookup"><span data-stu-id="31777-122">denied</span></span>|<span data-ttu-id="31777-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="31777-123">Boolean</span></span>|<span data-ttu-id="31777-124">Se verdadeiro, é negada proteção ou isenção ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="31777-124">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="31777-125">Relações</span><span class="sxs-lookup"><span data-stu-id="31777-125">Relationships</span></span>
<span data-ttu-id="31777-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="31777-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="31777-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="31777-127">JSON Representation</span></span>
<span data-ttu-id="31777-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="31777-128">Here is a JSON representation of the resource.</span></span>
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



