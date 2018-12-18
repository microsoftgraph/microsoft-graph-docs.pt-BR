---
title: Tipo de recurso rolePermission
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: 0433c3f3a0ab3ef63fcd2a44776c083ddb5b91a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325673"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="6d50b-103">Tipo de recurso rolePermission</span><span class="sxs-lookup"><span data-stu-id="6d50b-103">rolePermission resource type</span></span>

> <span data-ttu-id="6d50b-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6d50b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6d50b-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6d50b-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="6d50b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d50b-106">Properties</span></span>
|<span data-ttu-id="6d50b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d50b-107">Property</span></span>|<span data-ttu-id="6d50b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d50b-108">Type</span></span>|<span data-ttu-id="6d50b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d50b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d50b-110">resourceActions</span><span class="sxs-lookup"><span data-stu-id="6d50b-110">resourceActions</span></span>|<span data-ttu-id="6d50b-111">Coleção [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="6d50b-111">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="6d50b-112">Ações</span><span class="sxs-lookup"><span data-stu-id="6d50b-112">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d50b-113">Relações</span><span class="sxs-lookup"><span data-stu-id="6d50b-113">Relationships</span></span>
<span data-ttu-id="6d50b-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6d50b-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6d50b-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d50b-115">JSON Representation</span></span>
<span data-ttu-id="6d50b-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6d50b-116">Here is a JSON representation of the resource.</span></span>
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



