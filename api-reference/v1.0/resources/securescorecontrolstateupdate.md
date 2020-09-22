---
title: tipo de recurso secureScoreControlStateUpdate
description: Este recurso contém o histórico dos Estados de controle atualizados pelo usuário (os Estados de controle incluem padrão, ignorado, terceiros, revisado).
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8f57c501ed2a4a47dbba163270feca8917fcce27
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984030"
---
#  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="3f9d8-103">tipo de recurso secureScoreControlStateUpdate</span><span class="sxs-lookup"><span data-stu-id="3f9d8-103">secureScoreControlStateUpdate resource type</span></span>

<span data-ttu-id="3f9d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f9d8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3f9d8-105">Contém o histórico dos Estados de controle atualizados pelo usuário (os Estados de controle incluem padrão, ignorado, terceiros, revisado).</span><span class="sxs-lookup"><span data-stu-id="3f9d8-105">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

## <a name="properties"></a><span data-ttu-id="3f9d8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3f9d8-106">Properties</span></span>

|<span data-ttu-id="3f9d8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f9d8-107">Property</span></span> |<span data-ttu-id="3f9d8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f9d8-108">Type</span></span> |<span data-ttu-id="3f9d8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f9d8-109">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="3f9d8-110">assignedTo</span><span class="sxs-lookup"><span data-stu-id="3f9d8-110">assignedTo</span></span>|<span data-ttu-id="3f9d8-111">String</span><span class="sxs-lookup"><span data-stu-id="3f9d8-111">String</span></span>|<span data-ttu-id="3f9d8-112">Atribui o controle ao usuário que executará a ação.</span><span class="sxs-lookup"><span data-stu-id="3f9d8-112">Assigns the control to the user who will take the action.</span></span> |
|<span data-ttu-id="3f9d8-113">comment</span><span class="sxs-lookup"><span data-stu-id="3f9d8-113">comment</span></span>|<span data-ttu-id="3f9d8-114">String</span><span class="sxs-lookup"><span data-stu-id="3f9d8-114">String</span></span>|<span data-ttu-id="3f9d8-115">Fornece comentários opcionais sobre o controle.</span><span class="sxs-lookup"><span data-stu-id="3f9d8-115">Provides optional comment about the control.</span></span> |
|<span data-ttu-id="3f9d8-116">state</span><span class="sxs-lookup"><span data-stu-id="3f9d8-116">state</span></span>|<span data-ttu-id="3f9d8-117">String</span><span class="sxs-lookup"><span data-stu-id="3f9d8-117">String</span></span>|<span data-ttu-id="3f9d8-118">Estado do controle, que pode ser modificado por meio de um comando PATCH (por exemplo, ignorado, terceiros).</span><span class="sxs-lookup"><span data-stu-id="3f9d8-118">State of the control, which can be modified via a PATCH command (for example, ignored, thirdParty).</span></span> |
|<span data-ttu-id="3f9d8-119">updatedBy</span><span class="sxs-lookup"><span data-stu-id="3f9d8-119">updatedBy</span></span>|<span data-ttu-id="3f9d8-120">String</span><span class="sxs-lookup"><span data-stu-id="3f9d8-120">String</span></span>|<span data-ttu-id="3f9d8-121">ID do usuário que atualizou o estado do locatário.</span><span class="sxs-lookup"><span data-stu-id="3f9d8-121">ID of the user who updated tenant state.</span></span> |
|<span data-ttu-id="3f9d8-122">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f9d8-122">updatedDateTime</span></span>|<span data-ttu-id="3f9d8-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f9d8-123">DateTimeOffset</span></span>|<span data-ttu-id="3f9d8-124">Hora em que o estado do controle foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="3f9d8-124">Time at which the control state was updated.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3f9d8-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3f9d8-125">JSON representation</span></span>
 <span data-ttu-id="3f9d8-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3f9d8-126">The following is a JSON representation of the resource.</span></span>
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

