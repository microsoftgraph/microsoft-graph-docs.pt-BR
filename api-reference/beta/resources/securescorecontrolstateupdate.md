---
title: " tipo de recurso de secureScoreControlStateUpdate"
description: Este recurso contém o histórico de estados de controle atualizado por usuário (incluem de estados de controle padrão, Ignored, ThirdParty, revisado).
localization_priority: Normal
ms.openlocfilehash: 8d8c3122a6263ebc7b10b5edfb823953e2d587fc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888918"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="7b369-103">tipo de recurso de secureScoreControlStateUpdate</span><span class="sxs-lookup"><span data-stu-id="7b369-103">secureScoreControlStateUpdate resource type</span></span>
<span data-ttu-id="7b369-104">Contém o histórico dos Estados controle atualizados pelo usuário (incluem de estados de controle padrão, Ignored, ThirdParty, revisado).</span><span class="sxs-lookup"><span data-stu-id="7b369-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="7b369-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b369-105">Property</span></span> |<span data-ttu-id="7b369-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b369-106">Type</span></span> |<span data-ttu-id="7b369-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b369-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="7b369-108">assignedTo</span><span class="sxs-lookup"><span data-stu-id="7b369-108">assignedTo</span></span> | <span data-ttu-id="7b369-109">string</span><span class="sxs-lookup"><span data-stu-id="7b369-109">string</span></span> | <span data-ttu-id="7b369-110">Atribua o controle ao usuário que executará a ação</span><span class="sxs-lookup"><span data-stu-id="7b369-110">Assign the control to the user who will take the action</span></span> |
|<span data-ttu-id="7b369-111">comment</span><span class="sxs-lookup"><span data-stu-id="7b369-111">comment</span></span> | <span data-ttu-id="7b369-112">string</span><span class="sxs-lookup"><span data-stu-id="7b369-112">string</span></span> | <span data-ttu-id="7b369-113">Fornece um comentário opcional sobre o controle</span><span class="sxs-lookup"><span data-stu-id="7b369-113">Provides optional comment about the control</span></span> |
|<span data-ttu-id="7b369-114">estado</span><span class="sxs-lookup"><span data-stu-id="7b369-114">state</span></span> | <span data-ttu-id="7b369-115">string</span><span class="sxs-lookup"><span data-stu-id="7b369-115">string</span></span> | <span data-ttu-id="7b369-116">Estado do controle pode ser modificado usando-se o comando de PATCH (ex.: ignorados, thirdParty etc.)</span><span class="sxs-lookup"><span data-stu-id="7b369-116">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
|<span data-ttu-id="7b369-117">updatedBy</span><span class="sxs-lookup"><span data-stu-id="7b369-117">updatedBy</span></span> | <span data-ttu-id="7b369-118">string</span><span class="sxs-lookup"><span data-stu-id="7b369-118">string</span></span> |<span data-ttu-id="7b369-119">ID do usuário que atualizou o estado de locatário</span><span class="sxs-lookup"><span data-stu-id="7b369-119">ID of the user who updated tenant state</span></span> |
|<span data-ttu-id="7b369-120">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7b369-120">updatedDateTime</span></span> | <span data-ttu-id="7b369-121">DateTimeOffset?</span><span class="sxs-lookup"><span data-stu-id="7b369-121">DateTimeOffset?</span></span> |<span data-ttu-id="7b369-122">Tempo no qual controle estado foi atualizado</span><span class="sxs-lookup"><span data-stu-id="7b369-122">Time at which control state was updated</span></span> |
 ## <a name="json-representation"></a><span data-ttu-id="7b369-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b369-123">JSON representation</span></span>
 <span data-ttu-id="7b369-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7b369-124">The following is a JSON representation of the resource.</span></span>
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
