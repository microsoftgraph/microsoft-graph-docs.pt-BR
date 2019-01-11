---
title: Tipo de recurso rolePermission
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0669a0e169a71ea3806b21a125a4921b5161d516
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855570"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="3e0df-103">Tipo de recurso rolePermission</span><span class="sxs-lookup"><span data-stu-id="3e0df-103">rolePermission resource type</span></span>

> <span data-ttu-id="3e0df-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3e0df-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e0df-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3e0df-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e0df-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3e0df-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e0df-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3e0df-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="3e0df-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3e0df-108">Properties</span></span>
|<span data-ttu-id="3e0df-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3e0df-109">Property</span></span>|<span data-ttu-id="3e0df-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e0df-110">Type</span></span>|<span data-ttu-id="3e0df-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e0df-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e0df-112">actions</span><span class="sxs-lookup"><span data-stu-id="3e0df-112">actions</span></span>|<span data-ttu-id="3e0df-113">String collection</span><span class="sxs-lookup"><span data-stu-id="3e0df-113">String collection</span></span>|<span data-ttu-id="3e0df-114">Ações permitidas</span><span class="sxs-lookup"><span data-stu-id="3e0df-114">Allowed Actions</span></span>|
|<span data-ttu-id="3e0df-115">resourceActions</span><span class="sxs-lookup"><span data-stu-id="3e0df-115">resourceActions</span></span>|<span data-ttu-id="3e0df-116">Coleção [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="3e0df-116">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="3e0df-117">Ações</span><span class="sxs-lookup"><span data-stu-id="3e0df-117">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e0df-118">Relações</span><span class="sxs-lookup"><span data-stu-id="3e0df-118">Relationships</span></span>
<span data-ttu-id="3e0df-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3e0df-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3e0df-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3e0df-120">JSON Representation</span></span>
<span data-ttu-id="3e0df-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3e0df-121">Here is a JSON representation of the resource.</span></span>
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





