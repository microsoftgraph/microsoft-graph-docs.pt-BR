---
title: Tipo de recurso rolePermission
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2573b2319d06d6d10d952d94c8fc0a17ab8a36dd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037097"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="bca23-103">Tipo de recurso rolePermission</span><span class="sxs-lookup"><span data-stu-id="bca23-103">rolePermission resource type</span></span>

> <span data-ttu-id="bca23-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bca23-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bca23-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bca23-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="bca23-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bca23-106">Properties</span></span>
|<span data-ttu-id="bca23-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bca23-107">Property</span></span>|<span data-ttu-id="bca23-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="bca23-108">Type</span></span>|<span data-ttu-id="bca23-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bca23-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bca23-110">resourceActions</span><span class="sxs-lookup"><span data-stu-id="bca23-110">resourceActions</span></span>|<span data-ttu-id="bca23-111">Coleção [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="bca23-111">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="bca23-112">Ações</span><span class="sxs-lookup"><span data-stu-id="bca23-112">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="bca23-113">Relações</span><span class="sxs-lookup"><span data-stu-id="bca23-113">Relationships</span></span>
<span data-ttu-id="bca23-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bca23-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bca23-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bca23-115">JSON Representation</span></span>
<span data-ttu-id="bca23-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bca23-116">Here is a JSON representation of the resource.</span></span>
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



