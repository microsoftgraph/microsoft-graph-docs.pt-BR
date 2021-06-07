---
title: Tipo de recurso windowsInformationProtectionApp
description: Aplicativo para proteção de informações do Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 03dd609b8bd2c1835665827fff2bd89f6e810d77
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751290"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="39be7-103">Tipo de recurso windowsInformationProtectionApp</span><span class="sxs-lookup"><span data-stu-id="39be7-103">windowsInformationProtectionApp resource type</span></span>

<span data-ttu-id="39be7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39be7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="39be7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="39be7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39be7-106">Aplicativo para proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="39be7-106">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="39be7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="39be7-107">Properties</span></span>
|<span data-ttu-id="39be7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39be7-108">Property</span></span>|<span data-ttu-id="39be7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="39be7-109">Type</span></span>|<span data-ttu-id="39be7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="39be7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39be7-111">displayName</span><span class="sxs-lookup"><span data-stu-id="39be7-111">displayName</span></span>|<span data-ttu-id="39be7-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39be7-112">String</span></span>|<span data-ttu-id="39be7-113">Nome de exibição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="39be7-113">App display name.</span></span>|
|<span data-ttu-id="39be7-114">descrição</span><span class="sxs-lookup"><span data-stu-id="39be7-114">description</span></span>|<span data-ttu-id="39be7-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39be7-115">String</span></span>|<span data-ttu-id="39be7-116">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="39be7-116">The app's description.</span></span>|
|<span data-ttu-id="39be7-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="39be7-117">publisherName</span></span>|<span data-ttu-id="39be7-118">String</span><span class="sxs-lookup"><span data-stu-id="39be7-118">String</span></span>|<span data-ttu-id="39be7-119">O nome do distribuidor</span><span class="sxs-lookup"><span data-stu-id="39be7-119">The publisher name</span></span>|
|<span data-ttu-id="39be7-120">productName</span><span class="sxs-lookup"><span data-stu-id="39be7-120">productName</span></span>|<span data-ttu-id="39be7-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="39be7-121">String</span></span>|<span data-ttu-id="39be7-122">O nome do produto.</span><span class="sxs-lookup"><span data-stu-id="39be7-122">The product name.</span></span>|
|<span data-ttu-id="39be7-123">negado</span><span class="sxs-lookup"><span data-stu-id="39be7-123">denied</span></span>|<span data-ttu-id="39be7-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="39be7-124">Boolean</span></span>|<span data-ttu-id="39be7-125">Se verdadeiro, é negada proteção ou isenção ao aplicativo.</span><span class="sxs-lookup"><span data-stu-id="39be7-125">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39be7-126">Relações</span><span class="sxs-lookup"><span data-stu-id="39be7-126">Relationships</span></span>
<span data-ttu-id="39be7-127">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="39be7-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="39be7-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="39be7-128">JSON Representation</span></span>
<span data-ttu-id="39be7-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="39be7-129">Here is a JSON representation of the resource.</span></span>
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




