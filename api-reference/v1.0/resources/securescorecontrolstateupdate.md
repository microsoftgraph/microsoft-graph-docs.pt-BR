---
title: tipo de recurso secureScoreControlStateUpdate
description: Este recurso contém o histórico dos Estados de controle atualizados pelo usuário (os Estados de controle incluem padrão, ignorado, terceiros, revisado).
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9e051f2c4319a2b2ae1e3dbd9ba633785a345c4a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034472"
---
#  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="1e1b4-103">tipo de recurso secureScoreControlStateUpdate</span><span class="sxs-lookup"><span data-stu-id="1e1b4-103">secureScoreControlStateUpdate resource type</span></span>

<span data-ttu-id="1e1b4-104">Contém o histórico dos Estados de controle atualizados pelo usuário (os Estados de controle incluem padrão, ignorado, terceiros, revisado).</span><span class="sxs-lookup"><span data-stu-id="1e1b4-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

## <a name="properties"></a><span data-ttu-id="1e1b4-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1e1b4-105">Properties</span></span>

|<span data-ttu-id="1e1b4-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e1b4-106">Property</span></span> |<span data-ttu-id="1e1b4-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e1b4-107">Type</span></span> |<span data-ttu-id="1e1b4-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e1b4-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="1e1b4-109">assignedTo</span><span class="sxs-lookup"><span data-stu-id="1e1b4-109">assignedTo</span></span>|<span data-ttu-id="1e1b4-110">String</span><span class="sxs-lookup"><span data-stu-id="1e1b4-110">String</span></span>|<span data-ttu-id="1e1b4-111">Atribui o controle ao usuário que executará a ação.</span><span class="sxs-lookup"><span data-stu-id="1e1b4-111">Assigns the control to the user who will take the action.</span></span> |
|<span data-ttu-id="1e1b4-112">comment</span><span class="sxs-lookup"><span data-stu-id="1e1b4-112">comment</span></span>|<span data-ttu-id="1e1b4-113">String</span><span class="sxs-lookup"><span data-stu-id="1e1b4-113">String</span></span>|<span data-ttu-id="1e1b4-114">Fornece comentários opcionais sobre o controle.</span><span class="sxs-lookup"><span data-stu-id="1e1b4-114">Provides optional comment about the control.</span></span> |
|<span data-ttu-id="1e1b4-115">state</span><span class="sxs-lookup"><span data-stu-id="1e1b4-115">state</span></span>|<span data-ttu-id="1e1b4-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e1b4-116">String</span></span>|<span data-ttu-id="1e1b4-117">Estado do controle, que pode ser modificado por meio de um comando PATCH (por exemplo, ignorado, terceiros).</span><span class="sxs-lookup"><span data-stu-id="1e1b4-117">State of the control, which can be modified via a PATCH command (for example, ignored, thirdParty).</span></span> |
|<span data-ttu-id="1e1b4-118">updatedBy</span><span class="sxs-lookup"><span data-stu-id="1e1b4-118">updatedBy</span></span>|<span data-ttu-id="1e1b4-119">String</span><span class="sxs-lookup"><span data-stu-id="1e1b4-119">String</span></span>|<span data-ttu-id="1e1b4-120">ID do usuário que atualizou o estado do locatário.</span><span class="sxs-lookup"><span data-stu-id="1e1b4-120">ID of the user who updated tenant state.</span></span> |
|<span data-ttu-id="1e1b4-121">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e1b4-121">updatedDateTime</span></span>|<span data-ttu-id="1e1b4-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e1b4-122">DateTimeOffset</span></span>|<span data-ttu-id="1e1b4-123">Hora em que o estado do controle foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="1e1b4-123">Time at which the control state was updated.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1e1b4-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1e1b4-124">JSON representation</span></span>
 <span data-ttu-id="1e1b4-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1e1b4-125">The following is a JSON representation of the resource.</span></span>
 <!-- {
  "blockType": "resource",
  "optionalProperties": [
    
   ],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
 ```json
{
  "assignedTo": "String",
  "comment": "String",
  "state": "String",
  "updatedBy": "String",
  "updatedDateTime": "String (timestamp)"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
