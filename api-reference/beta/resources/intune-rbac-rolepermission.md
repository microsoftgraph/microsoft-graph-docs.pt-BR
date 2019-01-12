---
title: Tipo de recurso rolePermission
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c9a1ccacc4de13574ea984977dbfb05c09a2cea5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912327"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="8a4e9-103">Tipo de recurso rolePermission</span><span class="sxs-lookup"><span data-stu-id="8a4e9-103">rolePermission resource type</span></span>

> <span data-ttu-id="8a4e9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8a4e9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a4e9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8a4e9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8a4e9-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8a4e9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8a4e9-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8a4e9-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="8a4e9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8a4e9-108">Properties</span></span>
|<span data-ttu-id="8a4e9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8a4e9-109">Property</span></span>|<span data-ttu-id="8a4e9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a4e9-110">Type</span></span>|<span data-ttu-id="8a4e9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a4e9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a4e9-112">actions</span><span class="sxs-lookup"><span data-stu-id="8a4e9-112">actions</span></span>|<span data-ttu-id="8a4e9-113">String collection</span><span class="sxs-lookup"><span data-stu-id="8a4e9-113">String collection</span></span>|<span data-ttu-id="8a4e9-114">Ações permitidas</span><span class="sxs-lookup"><span data-stu-id="8a4e9-114">Allowed Actions</span></span>|
|<span data-ttu-id="8a4e9-115">resourceActions</span><span class="sxs-lookup"><span data-stu-id="8a4e9-115">resourceActions</span></span>|<span data-ttu-id="8a4e9-116">Coleção [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="8a4e9-116">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="8a4e9-117">Ações</span><span class="sxs-lookup"><span data-stu-id="8a4e9-117">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a4e9-118">Relações</span><span class="sxs-lookup"><span data-stu-id="8a4e9-118">Relationships</span></span>
<span data-ttu-id="8a4e9-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8a4e9-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8a4e9-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8a4e9-120">JSON Representation</span></span>
<span data-ttu-id="8a4e9-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8a4e9-121">Here is a JSON representation of the resource.</span></span>
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





