---
title: Tipo de recurso rolePermission
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3e284198b7b2e6ad3fe120bd1c17c96a1872b793
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816601"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="90227-103">Tipo de recurso rolePermission</span><span class="sxs-lookup"><span data-stu-id="90227-103">rolePermission resource type</span></span>

> <span data-ttu-id="90227-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="90227-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="90227-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="90227-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="90227-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="90227-106">Properties</span></span>
|<span data-ttu-id="90227-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90227-107">Property</span></span>|<span data-ttu-id="90227-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="90227-108">Type</span></span>|<span data-ttu-id="90227-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="90227-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90227-110">resourceActions</span><span class="sxs-lookup"><span data-stu-id="90227-110">resourceActions</span></span>|<span data-ttu-id="90227-111">Coleção [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="90227-111">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="90227-112">Ações</span><span class="sxs-lookup"><span data-stu-id="90227-112">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="90227-113">Relações</span><span class="sxs-lookup"><span data-stu-id="90227-113">Relationships</span></span>
<span data-ttu-id="90227-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="90227-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="90227-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="90227-115">JSON Representation</span></span>
<span data-ttu-id="90227-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="90227-116">Here is a JSON representation of the resource.</span></span>
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



