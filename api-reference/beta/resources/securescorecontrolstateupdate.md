---
title: " tipo de recurso de secureScoreControlStateUpdate"
description: Este recurso contém o histórico de estados de controle atualizado por usuário (incluem de estados de controle padrão, Ignored, ThirdParty, revisado).
localization_priority: Normal
ms.openlocfilehash: 8d8c3122a6263ebc7b10b5edfb823953e2d587fc
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641726"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="0d314-103">tipo de recurso de secureScoreControlStateUpdate</span><span class="sxs-lookup"><span data-stu-id="0d314-103">secureScoreControlStateUpdate resource type</span></span>
<span data-ttu-id="0d314-104">Contém o histórico dos Estados controle atualizados pelo usuário (incluem de estados de controle padrão, Ignored, ThirdParty, revisado).</span><span class="sxs-lookup"><span data-stu-id="0d314-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="0d314-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d314-105">Property</span></span> |<span data-ttu-id="0d314-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d314-106">Type</span></span> |<span data-ttu-id="0d314-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d314-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="0d314-108">assignedTo</span><span class="sxs-lookup"><span data-stu-id="0d314-108">assignedTo</span></span> | <span data-ttu-id="0d314-109">string</span><span class="sxs-lookup"><span data-stu-id="0d314-109">string</span></span> | <span data-ttu-id="0d314-110">Atribua o controle ao usuário que executará a ação</span><span class="sxs-lookup"><span data-stu-id="0d314-110">Assign the control to the user who will take the action</span></span> |
|<span data-ttu-id="0d314-111">comment</span><span class="sxs-lookup"><span data-stu-id="0d314-111">comment</span></span> | <span data-ttu-id="0d314-112">string</span><span class="sxs-lookup"><span data-stu-id="0d314-112">string</span></span> | <span data-ttu-id="0d314-113">Fornece um comentário opcional sobre o controle</span><span class="sxs-lookup"><span data-stu-id="0d314-113">Provides optional comment about the control</span></span> |
|<span data-ttu-id="0d314-114">state</span><span class="sxs-lookup"><span data-stu-id="0d314-114">state</span></span> | <span data-ttu-id="0d314-115">string</span><span class="sxs-lookup"><span data-stu-id="0d314-115">string</span></span> | <span data-ttu-id="0d314-116">Estado do controle pode ser modificado usando-se o comando de PATCH (ex.: ignorados, thirdParty etc.)</span><span class="sxs-lookup"><span data-stu-id="0d314-116">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
|<span data-ttu-id="0d314-117">updatedBy</span><span class="sxs-lookup"><span data-stu-id="0d314-117">updatedBy</span></span> | <span data-ttu-id="0d314-118">string</span><span class="sxs-lookup"><span data-stu-id="0d314-118">string</span></span> |<span data-ttu-id="0d314-119">ID do usuário que atualizou o estado de locatário</span><span class="sxs-lookup"><span data-stu-id="0d314-119">ID of the user who updated tenant state</span></span> |
|<span data-ttu-id="0d314-120">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d314-120">updatedDateTime</span></span> | <span data-ttu-id="0d314-121">DateTimeOffset?</span><span class="sxs-lookup"><span data-stu-id="0d314-121">DateTimeOffset?</span></span> |<span data-ttu-id="0d314-122">Tempo no qual controle estado foi atualizado</span><span class="sxs-lookup"><span data-stu-id="0d314-122">Time at which control state was updated</span></span> |
 ## <a name="json-representation"></a><span data-ttu-id="0d314-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0d314-123">JSON representation</span></span>
 <span data-ttu-id="0d314-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0d314-124">The following is a JSON representation of the resource.</span></span>
 <!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
 ```json
{
  "assignedTo": "String",
  "comment": "Double",
  "state": "Double",
  "updatedBy": "Double",
  "updatedDateTime": "Double"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
