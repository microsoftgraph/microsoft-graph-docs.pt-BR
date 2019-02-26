---
title: Tipo de recurso rolePermission
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a90de4e78bbc831ebb9eb7bf5ee65c26434fc06
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257782"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="15577-103">Tipo de recurso rolePermission</span><span class="sxs-lookup"><span data-stu-id="15577-103">rolePermission resource type</span></span>

> <span data-ttu-id="15577-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="15577-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15577-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="15577-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="15577-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="15577-106">Properties</span></span>
|<span data-ttu-id="15577-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15577-107">Property</span></span>|<span data-ttu-id="15577-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="15577-108">Type</span></span>|<span data-ttu-id="15577-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="15577-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15577-110">resourceActions</span><span class="sxs-lookup"><span data-stu-id="15577-110">resourceActions</span></span>|<span data-ttu-id="15577-111">Coleção [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="15577-111">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="15577-112">Ações</span><span class="sxs-lookup"><span data-stu-id="15577-112">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="15577-113">Relações</span><span class="sxs-lookup"><span data-stu-id="15577-113">Relationships</span></span>
<span data-ttu-id="15577-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="15577-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="15577-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="15577-115">JSON Representation</span></span>
<span data-ttu-id="15577-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="15577-116">Here is a JSON representation of the resource.</span></span>
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



