---
title: Tipo de recurso rolePermission
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: c33af6af3bc06a53bd24ddf97576551a5eea6e9c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349102"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="04bdc-103">Tipo de recurso rolePermission</span><span class="sxs-lookup"><span data-stu-id="04bdc-103">rolePermission resource type</span></span>

> <span data-ttu-id="04bdc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="04bdc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04bdc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="04bdc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04bdc-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="04bdc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04bdc-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="04bdc-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="04bdc-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04bdc-108">Properties</span></span>
|<span data-ttu-id="04bdc-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04bdc-109">Property</span></span>|<span data-ttu-id="04bdc-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="04bdc-110">Type</span></span>|<span data-ttu-id="04bdc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="04bdc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04bdc-112">actions</span><span class="sxs-lookup"><span data-stu-id="04bdc-112">actions</span></span>|<span data-ttu-id="04bdc-113">String collection</span><span class="sxs-lookup"><span data-stu-id="04bdc-113">String collection</span></span>|<span data-ttu-id="04bdc-114">Ações permitidas</span><span class="sxs-lookup"><span data-stu-id="04bdc-114">Allowed Actions</span></span>|
|<span data-ttu-id="04bdc-115">resourceActions</span><span class="sxs-lookup"><span data-stu-id="04bdc-115">resourceActions</span></span>|<span data-ttu-id="04bdc-116">Coleção [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="04bdc-116">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="04bdc-117">Ações</span><span class="sxs-lookup"><span data-stu-id="04bdc-117">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="04bdc-118">Relações</span><span class="sxs-lookup"><span data-stu-id="04bdc-118">Relationships</span></span>
<span data-ttu-id="04bdc-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="04bdc-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="04bdc-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04bdc-120">JSON Representation</span></span>
<span data-ttu-id="04bdc-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="04bdc-121">Here is a JSON representation of the resource.</span></span>
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





