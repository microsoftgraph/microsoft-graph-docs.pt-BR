---
title: Tipo de recurso rolePermission
description: Contém o conjunto de ResourceActions que determina as permissões permitidas e não permitidas para cada função.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 85370ad155d769d74f29dec80a03d3203feac8fa
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43356857"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="5cd39-103">Tipo de recurso rolePermission</span><span class="sxs-lookup"><span data-stu-id="5cd39-103">rolePermission resource type</span></span>

<span data-ttu-id="5cd39-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cd39-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5cd39-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5cd39-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5cd39-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5cd39-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cd39-107">Contém o conjunto de ResourceActions que determina as permissões permitidas e não permitidas para cada função.</span><span class="sxs-lookup"><span data-stu-id="5cd39-107">Contains the set of ResourceActions determining the allowed and not allowed permissions for each role.</span></span>

## <a name="properties"></a><span data-ttu-id="5cd39-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5cd39-108">Properties</span></span>
|<span data-ttu-id="5cd39-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5cd39-109">Property</span></span>|<span data-ttu-id="5cd39-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5cd39-110">Type</span></span>|<span data-ttu-id="5cd39-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5cd39-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cd39-112">actions</span><span class="sxs-lookup"><span data-stu-id="5cd39-112">actions</span></span>|<span data-ttu-id="5cd39-113">Coleção String</span><span class="sxs-lookup"><span data-stu-id="5cd39-113">String collection</span></span>|<span data-ttu-id="5cd39-114">Ações permitidas-preteridas</span><span class="sxs-lookup"><span data-stu-id="5cd39-114">Allowed Actions - Deprecated</span></span>|
|<span data-ttu-id="5cd39-115">resourceActions</span><span class="sxs-lookup"><span data-stu-id="5cd39-115">resourceActions</span></span>|<span data-ttu-id="5cd39-116">Coleção [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="5cd39-116">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="5cd39-117">Ações de recurso que contêm um conjunto de permissões permitidas e não permitidas.</span><span class="sxs-lookup"><span data-stu-id="5cd39-117">Resource Actions each containing a set of allowed and not allowed permissions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cd39-118">Relações</span><span class="sxs-lookup"><span data-stu-id="5cd39-118">Relationships</span></span>
<span data-ttu-id="5cd39-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5cd39-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5cd39-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5cd39-120">JSON Representation</span></span>
<span data-ttu-id="5cd39-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5cd39-121">Here is a JSON representation of the resource.</span></span>
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



