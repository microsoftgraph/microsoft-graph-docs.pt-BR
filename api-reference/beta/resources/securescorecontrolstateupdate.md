---
title: " tipo de recurso secureScoreControlStateUpdate"
description: Este recurso contém o histórico de Estados de controle atualizados pelo usuário (os Estados de controle incluem Default, ignorado, terceiros).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: f3b69838a6de68938efac12acdfbcd4fd977c684
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810402"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="43f83-103">tipo de recurso secureScoreControlStateUpdate</span><span class="sxs-lookup"><span data-stu-id="43f83-103">secureScoreControlStateUpdate resource type</span></span>
<span data-ttu-id="43f83-104">Contém o histórico dos Estados de controle atualizados pelo usuário (os Estados de controle incluem padrão, ignorado, terceiros, revisado).</span><span class="sxs-lookup"><span data-stu-id="43f83-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="43f83-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43f83-105">Property</span></span> |<span data-ttu-id="43f83-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="43f83-106">Type</span></span> |<span data-ttu-id="43f83-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="43f83-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="43f83-108">assignedTo</span><span class="sxs-lookup"><span data-stu-id="43f83-108">assignedTo</span></span> | <span data-ttu-id="43f83-109">string</span><span class="sxs-lookup"><span data-stu-id="43f83-109">string</span></span> | <span data-ttu-id="43f83-110">Atribuir o controle ao usuário que executará a ação</span><span class="sxs-lookup"><span data-stu-id="43f83-110">Assign the control to the user who will take the action</span></span> |
|<span data-ttu-id="43f83-111">comment</span><span class="sxs-lookup"><span data-stu-id="43f83-111">comment</span></span> | <span data-ttu-id="43f83-112">string</span><span class="sxs-lookup"><span data-stu-id="43f83-112">string</span></span> | <span data-ttu-id="43f83-113">Fornece comentários opcionais sobre o controle</span><span class="sxs-lookup"><span data-stu-id="43f83-113">Provides optional comment about the control</span></span> |
|<span data-ttu-id="43f83-114">estado</span><span class="sxs-lookup"><span data-stu-id="43f83-114">state</span></span> | <span data-ttu-id="43f83-115">string</span><span class="sxs-lookup"><span data-stu-id="43f83-115">string</span></span> | <span data-ttu-id="43f83-116">O estado do controle pode ser modificado usando o comando PATCH (ex: ignorado, terceiros etc.)</span><span class="sxs-lookup"><span data-stu-id="43f83-116">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
|<span data-ttu-id="43f83-117">updatedBy</span><span class="sxs-lookup"><span data-stu-id="43f83-117">updatedBy</span></span> | <span data-ttu-id="43f83-118">string</span><span class="sxs-lookup"><span data-stu-id="43f83-118">string</span></span> |<span data-ttu-id="43f83-119">ID do usuário que atualizou o estado do locatário</span><span class="sxs-lookup"><span data-stu-id="43f83-119">ID of the user who updated tenant state</span></span> |
|<span data-ttu-id="43f83-120">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="43f83-120">updatedDateTime</span></span> | <span data-ttu-id="43f83-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43f83-121">DateTimeOffset</span></span> |<span data-ttu-id="43f83-122">Hora em que o estado de controle foi atualizado</span><span class="sxs-lookup"><span data-stu-id="43f83-122">Time at which control state was updated</span></span> |
 ## <a name="json-representation"></a><span data-ttu-id="43f83-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="43f83-123">JSON representation</span></span>
 <span data-ttu-id="43f83-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="43f83-124">The following is a JSON representation of the resource.</span></span>
 <!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
 ```json
{
  "assignedTo": "String",
  "comment": "string",
  "state": "string",
  "updatedBy": "string",
  "updatedDateTime": "DateTimeOffset"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
