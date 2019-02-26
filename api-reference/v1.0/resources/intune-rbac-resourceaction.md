---
title: Tipo de recurso resourceAction
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a48d09d8aeadc9a5d60559d25a4bdcc322d10f21
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262178"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="40dbe-103">Tipo de recurso resourceAction</span><span class="sxs-lookup"><span data-stu-id="40dbe-103">resourceAction resource type</span></span>

> <span data-ttu-id="40dbe-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="40dbe-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40dbe-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="40dbe-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="40dbe-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="40dbe-106">Properties</span></span>
|<span data-ttu-id="40dbe-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40dbe-107">Property</span></span>|<span data-ttu-id="40dbe-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="40dbe-108">Type</span></span>|<span data-ttu-id="40dbe-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="40dbe-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40dbe-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="40dbe-110">allowedResourceActions</span></span>|<span data-ttu-id="40dbe-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="40dbe-111">String collection</span></span>|<span data-ttu-id="40dbe-112">Ações permitidas</span><span class="sxs-lookup"><span data-stu-id="40dbe-112">Allowed Actions</span></span>|
|<span data-ttu-id="40dbe-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="40dbe-113">notAllowedResourceActions</span></span>|<span data-ttu-id="40dbe-114">String collection</span><span class="sxs-lookup"><span data-stu-id="40dbe-114">String collection</span></span>|<span data-ttu-id="40dbe-115">Ações não permitidas</span><span class="sxs-lookup"><span data-stu-id="40dbe-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="40dbe-116">Relações</span><span class="sxs-lookup"><span data-stu-id="40dbe-116">Relationships</span></span>
<span data-ttu-id="40dbe-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="40dbe-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="40dbe-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="40dbe-118">JSON Representation</span></span>
<span data-ttu-id="40dbe-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="40dbe-119">Here is a JSON representation of the resource.</span></span>
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



