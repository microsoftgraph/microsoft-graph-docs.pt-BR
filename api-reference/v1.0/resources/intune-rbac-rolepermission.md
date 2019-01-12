---
title: Tipo de recurso rolePermission
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b8b9ba237052fef2b4caa8123d147ea1782fa9b9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932802"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="270d6-103">Tipo de recurso rolePermission</span><span class="sxs-lookup"><span data-stu-id="270d6-103">rolePermission resource type</span></span>

> <span data-ttu-id="270d6-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="270d6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="270d6-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="270d6-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="270d6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="270d6-106">Properties</span></span>
|<span data-ttu-id="270d6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="270d6-107">Property</span></span>|<span data-ttu-id="270d6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="270d6-108">Type</span></span>|<span data-ttu-id="270d6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="270d6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="270d6-110">resourceActions</span><span class="sxs-lookup"><span data-stu-id="270d6-110">resourceActions</span></span>|<span data-ttu-id="270d6-111">Coleção [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="270d6-111">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="270d6-112">Ações</span><span class="sxs-lookup"><span data-stu-id="270d6-112">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="270d6-113">Relações</span><span class="sxs-lookup"><span data-stu-id="270d6-113">Relationships</span></span>
<span data-ttu-id="270d6-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="270d6-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="270d6-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="270d6-115">JSON Representation</span></span>
<span data-ttu-id="270d6-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="270d6-116">Here is a JSON representation of the resource.</span></span>
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



