---
title: Tipo de recurso iosMinimumOperatingSystem
description: Contém as propriedades do sistema operacional mínimo obrigatório para um aplicativo móvel iOS.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 43409d7c4f4eb7bedd4a169c5f56d969e2b9d03d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005937"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="11859-103">Tipo de recurso iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="11859-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="11859-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="11859-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11859-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="11859-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11859-106">Contém as propriedades do sistema operacional mínimo obrigatório para um aplicativo móvel iOS.</span><span class="sxs-lookup"><span data-stu-id="11859-106">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="11859-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11859-107">Properties</span></span>
|<span data-ttu-id="11859-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11859-108">Property</span></span>|<span data-ttu-id="11859-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="11859-109">Type</span></span>|<span data-ttu-id="11859-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="11859-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11859-111">v8_0</span><span class="sxs-lookup"><span data-stu-id="11859-111">v8_0</span></span>|<span data-ttu-id="11859-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="11859-112">Boolean</span></span>|<span data-ttu-id="11859-113">Versão 8.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="11859-113">Version 8.0 or later.</span></span>|
|<span data-ttu-id="11859-114">v9_0</span><span class="sxs-lookup"><span data-stu-id="11859-114">v9_0</span></span>|<span data-ttu-id="11859-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="11859-115">Boolean</span></span>|<span data-ttu-id="11859-116">Versão 9.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="11859-116">Version 9.0 or later.</span></span>|
|<span data-ttu-id="11859-117">v10_0</span><span class="sxs-lookup"><span data-stu-id="11859-117">v10_0</span></span>|<span data-ttu-id="11859-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="11859-118">Boolean</span></span>|<span data-ttu-id="11859-119">Versão 10.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="11859-119">Version 10.0 or later.</span></span>|
|<span data-ttu-id="11859-120">v11_0</span><span class="sxs-lookup"><span data-stu-id="11859-120">v11_0</span></span>|<span data-ttu-id="11859-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="11859-121">Boolean</span></span>|<span data-ttu-id="11859-122">Versão 11.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="11859-122">Version 11.0 or later.</span></span>|
|<span data-ttu-id="11859-123">v12_0</span><span class="sxs-lookup"><span data-stu-id="11859-123">v12_0</span></span>|<span data-ttu-id="11859-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="11859-124">Boolean</span></span>|<span data-ttu-id="11859-125">Versão 12,0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="11859-125">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11859-126">Relações</span><span class="sxs-lookup"><span data-stu-id="11859-126">Relationships</span></span>
<span data-ttu-id="11859-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="11859-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="11859-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11859-128">JSON Representation</span></span>
<span data-ttu-id="11859-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="11859-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMinimumOperatingSystem",
  "v8_0": true,
  "v9_0": true,
  "v10_0": true,
  "v11_0": true,
  "v12_0": true
}
```





