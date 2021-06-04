---
title: Tipo de recurso rolePermission
description: Contém o conjunto de ResourceActions que determina as permissões permitidas e não permitidas para cada função.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7598e7f7a54910d706ec95741234a38a9a9ba422
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752746"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="acf08-103">Tipo de recurso rolePermission</span><span class="sxs-lookup"><span data-stu-id="acf08-103">rolePermission resource type</span></span>

<span data-ttu-id="acf08-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acf08-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="acf08-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="acf08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="acf08-106">Contém o conjunto de ResourceActions que determina as permissões permitidas e não permitidas para cada função.</span><span class="sxs-lookup"><span data-stu-id="acf08-106">Contains the set of ResourceActions determining the allowed and not allowed permissions for each role.</span></span>

## <a name="properties"></a><span data-ttu-id="acf08-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="acf08-107">Properties</span></span>
|<span data-ttu-id="acf08-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="acf08-108">Property</span></span>|<span data-ttu-id="acf08-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="acf08-109">Type</span></span>|<span data-ttu-id="acf08-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="acf08-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acf08-111">resourceActions</span><span class="sxs-lookup"><span data-stu-id="acf08-111">resourceActions</span></span>|<span data-ttu-id="acf08-112">Coleção [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="acf08-112">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="acf08-113">Ações de Recurso que contêm um conjunto de permissões permitidas e não permitidas.</span><span class="sxs-lookup"><span data-stu-id="acf08-113">Resource Actions each containing a set of allowed and not allowed permissions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="acf08-114">Relações</span><span class="sxs-lookup"><span data-stu-id="acf08-114">Relationships</span></span>
<span data-ttu-id="acf08-115">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="acf08-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="acf08-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="acf08-116">JSON Representation</span></span>
<span data-ttu-id="acf08-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="acf08-117">Here is a JSON representation of the resource.</span></span>
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




