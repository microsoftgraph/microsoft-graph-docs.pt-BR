---
title: Tipo de recurso rolePermission
description: Contém o conjunto de ResourceActions que determina as permissões permitidas e não permitidas para cada função.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2514200aec93288f1841190f0a0a5b3fdb556429
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725166"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="053f3-103">Tipo de recurso rolePermission</span><span class="sxs-lookup"><span data-stu-id="053f3-103">rolePermission resource type</span></span>

<span data-ttu-id="053f3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="053f3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="053f3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="053f3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="053f3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="053f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="053f3-107">Contém o conjunto de ResourceActions que determina as permissões permitidas e não permitidas para cada função.</span><span class="sxs-lookup"><span data-stu-id="053f3-107">Contains the set of ResourceActions determining the allowed and not allowed permissions for each role.</span></span>

## <a name="properties"></a><span data-ttu-id="053f3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="053f3-108">Properties</span></span>
|<span data-ttu-id="053f3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="053f3-109">Property</span></span>|<span data-ttu-id="053f3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="053f3-110">Type</span></span>|<span data-ttu-id="053f3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="053f3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="053f3-112">actions</span><span class="sxs-lookup"><span data-stu-id="053f3-112">actions</span></span>|<span data-ttu-id="053f3-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="053f3-113">String collection</span></span>|<span data-ttu-id="053f3-114">Ações permitidas-preteridas</span><span class="sxs-lookup"><span data-stu-id="053f3-114">Allowed Actions - Deprecated</span></span>|
|<span data-ttu-id="053f3-115">resourceActions</span><span class="sxs-lookup"><span data-stu-id="053f3-115">resourceActions</span></span>|<span data-ttu-id="053f3-116">Coleção [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="053f3-116">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="053f3-117">Ações de recurso que contêm um conjunto de permissões permitidas e não permitidas.</span><span class="sxs-lookup"><span data-stu-id="053f3-117">Resource Actions each containing a set of allowed and not allowed permissions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="053f3-118">Relações</span><span class="sxs-lookup"><span data-stu-id="053f3-118">Relationships</span></span>
<span data-ttu-id="053f3-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="053f3-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="053f3-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="053f3-120">JSON Representation</span></span>
<span data-ttu-id="053f3-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="053f3-121">Here is a JSON representation of the resource.</span></span>
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





