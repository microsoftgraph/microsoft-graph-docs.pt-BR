---
title: Tipo de recurso rolePermission
description: Contém o conjunto de ResourceActions que determina as permissões permitidas e não permitidas para cada função.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8cbe41bae81d165d0800a5184e1f7babedebc09d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993519"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="a877a-103">Tipo de recurso rolePermission</span><span class="sxs-lookup"><span data-stu-id="a877a-103">rolePermission resource type</span></span>

> <span data-ttu-id="a877a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a877a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a877a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a877a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a877a-106">Contém o conjunto de ResourceActions que determina as permissões permitidas e não permitidas para cada função.</span><span class="sxs-lookup"><span data-stu-id="a877a-106">Contains the set of ResourceActions determining the allowed and not allowed permissions for each role.</span></span>

## <a name="properties"></a><span data-ttu-id="a877a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a877a-107">Properties</span></span>
|<span data-ttu-id="a877a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a877a-108">Property</span></span>|<span data-ttu-id="a877a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a877a-109">Type</span></span>|<span data-ttu-id="a877a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a877a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a877a-111">actions</span><span class="sxs-lookup"><span data-stu-id="a877a-111">actions</span></span>|<span data-ttu-id="a877a-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="a877a-112">String collection</span></span>|<span data-ttu-id="a877a-113">Ações permitidas-preteridas</span><span class="sxs-lookup"><span data-stu-id="a877a-113">Allowed Actions - Deprecated</span></span>|
|<span data-ttu-id="a877a-114">resourceActions</span><span class="sxs-lookup"><span data-stu-id="a877a-114">resourceActions</span></span>|<span data-ttu-id="a877a-115">Coleção [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="a877a-115">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="a877a-116">Ações de recurso que contêm um conjunto de permissões permitidas e não permitidas.</span><span class="sxs-lookup"><span data-stu-id="a877a-116">Resource Actions each containing a set of allowed and not allowed permissions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a877a-117">Relações</span><span class="sxs-lookup"><span data-stu-id="a877a-117">Relationships</span></span>
<span data-ttu-id="a877a-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a877a-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a877a-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a877a-119">JSON Representation</span></span>
<span data-ttu-id="a877a-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a877a-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rolePermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rolePermission",
  "actions": [
    "String"
  ],
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





