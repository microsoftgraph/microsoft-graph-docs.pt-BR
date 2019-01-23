---
title: Tipo de recurso iosMinimumOperatingSystem
description: Contém as propriedades do sistema operacional mínimo obrigatório para um aplicativo móvel iOS.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d4a97932c76a737aa1a98321feb429244228c97d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406938"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="fbbe0-103">Tipo de recurso iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="fbbe0-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="fbbe0-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="fbbe0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fbbe0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fbbe0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fbbe0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="fbbe0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbbe0-107">Contém as propriedades do sistema operacional mínimo obrigatório para um aplicativo móvel iOS.</span><span class="sxs-lookup"><span data-stu-id="fbbe0-107">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="fbbe0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fbbe0-108">Properties</span></span>
|<span data-ttu-id="fbbe0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fbbe0-109">Property</span></span>|<span data-ttu-id="fbbe0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="fbbe0-110">Type</span></span>|<span data-ttu-id="fbbe0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fbbe0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbbe0-112">v8_0</span><span class="sxs-lookup"><span data-stu-id="fbbe0-112">v8_0</span></span>|<span data-ttu-id="fbbe0-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="fbbe0-113">Boolean</span></span>|<span data-ttu-id="fbbe0-114">Versão 8.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="fbbe0-114">Version 8.0 or later.</span></span>|
|<span data-ttu-id="fbbe0-115">v9_0</span><span class="sxs-lookup"><span data-stu-id="fbbe0-115">v9_0</span></span>|<span data-ttu-id="fbbe0-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="fbbe0-116">Boolean</span></span>|<span data-ttu-id="fbbe0-117">Versão 9.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="fbbe0-117">Version 9.0 or later.</span></span>|
|<span data-ttu-id="fbbe0-118">v10_0</span><span class="sxs-lookup"><span data-stu-id="fbbe0-118">v10_0</span></span>|<span data-ttu-id="fbbe0-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="fbbe0-119">Boolean</span></span>|<span data-ttu-id="fbbe0-120">Versão 10.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="fbbe0-120">Version 10.0 or later.</span></span>|
|<span data-ttu-id="fbbe0-121">v11_0</span><span class="sxs-lookup"><span data-stu-id="fbbe0-121">v11_0</span></span>|<span data-ttu-id="fbbe0-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="fbbe0-122">Boolean</span></span>|<span data-ttu-id="fbbe0-123">Versão 11.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="fbbe0-123">Version 11.0 or later.</span></span>|
|<span data-ttu-id="fbbe0-124">v12_0</span><span class="sxs-lookup"><span data-stu-id="fbbe0-124">v12_0</span></span>|<span data-ttu-id="fbbe0-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbbe0-125">Boolean</span></span>|<span data-ttu-id="fbbe0-126">Versão 12.0 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="fbbe0-126">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbbe0-127">Relações</span><span class="sxs-lookup"><span data-stu-id="fbbe0-127">Relationships</span></span>
<span data-ttu-id="fbbe0-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fbbe0-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fbbe0-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fbbe0-129">JSON Representation</span></span>
<span data-ttu-id="fbbe0-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fbbe0-130">Here is a JSON representation of the resource.</span></span>
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




