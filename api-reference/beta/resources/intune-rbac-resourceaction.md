---
title: Tipo de recurso resourceAction
description: Conjunto de ações permitidas e não permitidas para um recurso.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 597a9c7cdc2f04247e799772f100d1a0b778453e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939984"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="a8342-103">Tipo de recurso resourceAction</span><span class="sxs-lookup"><span data-stu-id="a8342-103">resourceAction resource type</span></span>

> <span data-ttu-id="a8342-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a8342-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8342-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a8342-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8342-106">Conjunto de ações permitidas e não permitidas para um recurso.</span><span class="sxs-lookup"><span data-stu-id="a8342-106">Set of allowed and not allowed actions for a resource.</span></span>

## <a name="properties"></a><span data-ttu-id="a8342-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8342-107">Properties</span></span>
|<span data-ttu-id="a8342-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a8342-108">Property</span></span>|<span data-ttu-id="a8342-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8342-109">Type</span></span>|<span data-ttu-id="a8342-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8342-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8342-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="a8342-111">allowedResourceActions</span></span>|<span data-ttu-id="a8342-112">String collection</span><span class="sxs-lookup"><span data-stu-id="a8342-112">String collection</span></span>|<span data-ttu-id="a8342-113">Ações permitidas</span><span class="sxs-lookup"><span data-stu-id="a8342-113">Allowed Actions</span></span>|
|<span data-ttu-id="a8342-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="a8342-114">notAllowedResourceActions</span></span>|<span data-ttu-id="a8342-115">String collection</span><span class="sxs-lookup"><span data-stu-id="a8342-115">String collection</span></span>|<span data-ttu-id="a8342-116">Ações não permitidas.</span><span class="sxs-lookup"><span data-stu-id="a8342-116">Not Allowed Actions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8342-117">Relações</span><span class="sxs-lookup"><span data-stu-id="a8342-117">Relationships</span></span>
<span data-ttu-id="a8342-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a8342-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8342-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8342-119">JSON Representation</span></span>
<span data-ttu-id="a8342-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8342-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```




