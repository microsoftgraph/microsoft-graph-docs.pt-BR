---
title: Tipo de recurso resourceAction
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a48d09d8aeadc9a5d60559d25a4bdcc322d10f21
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553887"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="89138-103">Tipo de recurso resourceAction</span><span class="sxs-lookup"><span data-stu-id="89138-103">resourceAction resource type</span></span>

> <span data-ttu-id="89138-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="89138-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89138-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="89138-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="89138-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="89138-106">Properties</span></span>
|<span data-ttu-id="89138-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89138-107">Property</span></span>|<span data-ttu-id="89138-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="89138-108">Type</span></span>|<span data-ttu-id="89138-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="89138-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89138-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="89138-110">allowedResourceActions</span></span>|<span data-ttu-id="89138-111">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="89138-111">String collection</span></span>|<span data-ttu-id="89138-112">Ações permitidas</span><span class="sxs-lookup"><span data-stu-id="89138-112">Allowed Actions</span></span>|
|<span data-ttu-id="89138-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="89138-113">notAllowedResourceActions</span></span>|<span data-ttu-id="89138-114">String collection</span><span class="sxs-lookup"><span data-stu-id="89138-114">String collection</span></span>|<span data-ttu-id="89138-115">Ações não permitidas</span><span class="sxs-lookup"><span data-stu-id="89138-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="89138-116">Relações</span><span class="sxs-lookup"><span data-stu-id="89138-116">Relationships</span></span>
<span data-ttu-id="89138-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="89138-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="89138-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="89138-118">JSON Representation</span></span>
<span data-ttu-id="89138-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="89138-119">Here is a JSON representation of the resource.</span></span>
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



