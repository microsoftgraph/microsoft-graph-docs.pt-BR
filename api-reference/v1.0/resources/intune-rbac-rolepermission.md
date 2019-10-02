---
title: Tipo de recurso rolePermission
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2f53a6250500137b368f17ae71524f4e1121d1aa
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355873"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="e1da5-103">Tipo de recurso rolePermission</span><span class="sxs-lookup"><span data-stu-id="e1da5-103">rolePermission resource type</span></span>

> <span data-ttu-id="e1da5-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1da5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1da5-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e1da5-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e1da5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1da5-106">Properties</span></span>
|<span data-ttu-id="e1da5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1da5-107">Property</span></span>|<span data-ttu-id="e1da5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1da5-108">Type</span></span>|<span data-ttu-id="e1da5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1da5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1da5-110">resourceActions</span><span class="sxs-lookup"><span data-stu-id="e1da5-110">resourceActions</span></span>|<span data-ttu-id="e1da5-111">Coleção [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="e1da5-111">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="e1da5-112">Ações</span><span class="sxs-lookup"><span data-stu-id="e1da5-112">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1da5-113">Relações</span><span class="sxs-lookup"><span data-stu-id="e1da5-113">Relationships</span></span>
<span data-ttu-id="e1da5-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1da5-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1da5-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1da5-115">JSON Representation</span></span>
<span data-ttu-id="e1da5-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1da5-116">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rolePermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rolePermission",
  "resourceActions": [
    {
      "@odata.type": "microsoft.graph.resourceAction",
      "allowedResourceActions": [
        "String"
      ],
      "notAllowedResourceActions": [
        "String"
      ]
    }
  ]
}
```




