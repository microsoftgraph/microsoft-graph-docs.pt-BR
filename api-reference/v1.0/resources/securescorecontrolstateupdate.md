---
title: tipo de recurso secureScoreControlStateUpdate
description: Este recurso contém o histórico dos Estados de controle atualizados pelo usuário (os Estados de controle incluem padrão, ignorado, terceiros, revisado).
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0fe88741da75718b1509fd4f8015a37fcf7828bf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446958"
---
#  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="8dbfb-103">tipo de recurso secureScoreControlStateUpdate</span><span class="sxs-lookup"><span data-stu-id="8dbfb-103">secureScoreControlStateUpdate resource type</span></span>

<span data-ttu-id="8dbfb-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8dbfb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8dbfb-105">Contém o histórico dos Estados de controle atualizados pelo usuário (os Estados de controle incluem padrão, ignorado, terceiros, revisado).</span><span class="sxs-lookup"><span data-stu-id="8dbfb-105">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

## <a name="properties"></a><span data-ttu-id="8dbfb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8dbfb-106">Properties</span></span>

|<span data-ttu-id="8dbfb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8dbfb-107">Property</span></span> |<span data-ttu-id="8dbfb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8dbfb-108">Type</span></span> |<span data-ttu-id="8dbfb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8dbfb-109">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="8dbfb-110">assignedTo</span><span class="sxs-lookup"><span data-stu-id="8dbfb-110">assignedTo</span></span>|<span data-ttu-id="8dbfb-111">String</span><span class="sxs-lookup"><span data-stu-id="8dbfb-111">String</span></span>|<span data-ttu-id="8dbfb-112">Atribui o controle ao usuário que executará a ação.</span><span class="sxs-lookup"><span data-stu-id="8dbfb-112">Assigns the control to the user who will take the action.</span></span> |
|<span data-ttu-id="8dbfb-113">comment</span><span class="sxs-lookup"><span data-stu-id="8dbfb-113">comment</span></span>|<span data-ttu-id="8dbfb-114">String</span><span class="sxs-lookup"><span data-stu-id="8dbfb-114">String</span></span>|<span data-ttu-id="8dbfb-115">Fornece comentários opcionais sobre o controle.</span><span class="sxs-lookup"><span data-stu-id="8dbfb-115">Provides optional comment about the control.</span></span> |
|<span data-ttu-id="8dbfb-116">state</span><span class="sxs-lookup"><span data-stu-id="8dbfb-116">state</span></span>|<span data-ttu-id="8dbfb-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8dbfb-117">String</span></span>|<span data-ttu-id="8dbfb-118">Estado do controle, que pode ser modificado por meio de um comando PATCH (por exemplo, ignorado, terceiros).</span><span class="sxs-lookup"><span data-stu-id="8dbfb-118">State of the control, which can be modified via a PATCH command (for example, ignored, thirdParty).</span></span> |
|<span data-ttu-id="8dbfb-119">updatedBy</span><span class="sxs-lookup"><span data-stu-id="8dbfb-119">updatedBy</span></span>|<span data-ttu-id="8dbfb-120">String</span><span class="sxs-lookup"><span data-stu-id="8dbfb-120">String</span></span>|<span data-ttu-id="8dbfb-121">ID do usuário que atualizou o estado do locatário.</span><span class="sxs-lookup"><span data-stu-id="8dbfb-121">ID of the user who updated tenant state.</span></span> |
|<span data-ttu-id="8dbfb-122">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="8dbfb-122">updatedDateTime</span></span>|<span data-ttu-id="8dbfb-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8dbfb-123">DateTimeOffset</span></span>|<span data-ttu-id="8dbfb-124">Hora em que o estado do controle foi atualizado.</span><span class="sxs-lookup"><span data-stu-id="8dbfb-124">Time at which the control state was updated.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8dbfb-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8dbfb-125">JSON representation</span></span>
 <span data-ttu-id="8dbfb-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8dbfb-126">The following is a JSON representation of the resource.</span></span>
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
