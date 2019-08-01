---
title: Tipo de recurso groupAssignmentTarget
description: Representa uma atribuição para um grupo.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 87e4e4707a1884e7d657bae9c6e41fee69dc831d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036915"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="43867-103">Tipo de recurso groupAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="43867-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="43867-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="43867-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43867-105">Representa uma atribuição para um grupo.</span><span class="sxs-lookup"><span data-stu-id="43867-105">Represents an assignment to a group.</span></span>


<span data-ttu-id="43867-106">Herda de [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="43867-106">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="43867-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="43867-107">Properties</span></span>
|<span data-ttu-id="43867-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43867-108">Property</span></span>|<span data-ttu-id="43867-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="43867-109">Type</span></span>|<span data-ttu-id="43867-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="43867-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43867-111">groupId</span><span class="sxs-lookup"><span data-stu-id="43867-111">groupId</span></span>|<span data-ttu-id="43867-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43867-112">String</span></span>|<span data-ttu-id="43867-113">A ID do Grupo que representa o destino da atribuição.</span><span class="sxs-lookup"><span data-stu-id="43867-113">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43867-114">Relações</span><span class="sxs-lookup"><span data-stu-id="43867-114">Relationships</span></span>
<span data-ttu-id="43867-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="43867-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="43867-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="43867-116">JSON Representation</span></span>
<span data-ttu-id="43867-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="43867-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupAssignmentTarget",
  "groupId": "String"
}
```



