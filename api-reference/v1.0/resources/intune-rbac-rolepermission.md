---
title: Tipo de recurso rolePermission
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7a8e607e01ab0b2955e8a016c0b9d73ee4748cbf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441584"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="20dd9-103">Tipo de recurso rolePermission</span><span class="sxs-lookup"><span data-stu-id="20dd9-103">rolePermission resource type</span></span>

<span data-ttu-id="20dd9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20dd9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="20dd9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="20dd9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20dd9-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="20dd9-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="20dd9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20dd9-107">Properties</span></span>
|<span data-ttu-id="20dd9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20dd9-108">Property</span></span>|<span data-ttu-id="20dd9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="20dd9-109">Type</span></span>|<span data-ttu-id="20dd9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="20dd9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20dd9-111">resourceActions</span><span class="sxs-lookup"><span data-stu-id="20dd9-111">resourceActions</span></span>|<span data-ttu-id="20dd9-112">Coleção [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="20dd9-112">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="20dd9-113">Ações</span><span class="sxs-lookup"><span data-stu-id="20dd9-113">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="20dd9-114">Relações</span><span class="sxs-lookup"><span data-stu-id="20dd9-114">Relationships</span></span>
<span data-ttu-id="20dd9-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="20dd9-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="20dd9-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="20dd9-116">JSON Representation</span></span>
<span data-ttu-id="20dd9-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="20dd9-117">Here is a JSON representation of the resource.</span></span>
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







