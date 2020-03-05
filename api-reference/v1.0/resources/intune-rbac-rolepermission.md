---
title: Tipo de recurso rolePermission
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f3a01bf7c6f607c7340cff8ea5075a24fb879ddb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447924"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="f8558-103">Tipo de recurso rolePermission</span><span class="sxs-lookup"><span data-stu-id="f8558-103">rolePermission resource type</span></span>

<span data-ttu-id="f8558-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f8558-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f8558-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f8558-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8558-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f8558-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f8558-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f8558-107">Properties</span></span>
|<span data-ttu-id="f8558-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8558-108">Property</span></span>|<span data-ttu-id="f8558-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8558-109">Type</span></span>|<span data-ttu-id="f8558-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8558-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8558-111">resourceActions</span><span class="sxs-lookup"><span data-stu-id="f8558-111">resourceActions</span></span>|<span data-ttu-id="f8558-112">Coleção [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="f8558-112">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="f8558-113">Ações</span><span class="sxs-lookup"><span data-stu-id="f8558-113">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8558-114">Relações</span><span class="sxs-lookup"><span data-stu-id="f8558-114">Relationships</span></span>
<span data-ttu-id="f8558-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f8558-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8558-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f8558-116">JSON Representation</span></span>
<span data-ttu-id="f8558-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f8558-117">Here is a JSON representation of the resource.</span></span>
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




