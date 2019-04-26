---
title: " tipo de recurso secureScoreControlStateUpdate"
description: Este recurso contém o histórico de Estados de controle atualizados pelo usuário (os Estados de controle incluem Default, ignorado, terceiros).
localization_priority: Normal
ms.openlocfilehash: 24febeb4bfb055e89e59cdb4f79c8b60c6c40347
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343357"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="81849-103">tipo de recurso secureScoreControlStateUpdate</span><span class="sxs-lookup"><span data-stu-id="81849-103">secureScoreControlStateUpdate resource type</span></span>
<span data-ttu-id="81849-104">Contém o histórico dos Estados de controle atualizados pelo usuário (os Estados de controle incluem padrão, ignorado, terceiros, reVisado).</span><span class="sxs-lookup"><span data-stu-id="81849-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="81849-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81849-105">Property</span></span> |<span data-ttu-id="81849-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="81849-106">Type</span></span> |<span data-ttu-id="81849-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="81849-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="81849-108">assignedTo</span><span class="sxs-lookup"><span data-stu-id="81849-108">assignedTo</span></span> | <span data-ttu-id="81849-109">string</span><span class="sxs-lookup"><span data-stu-id="81849-109">string</span></span> | <span data-ttu-id="81849-110">Atribuir o controle ao usuário que executará a ação</span><span class="sxs-lookup"><span data-stu-id="81849-110">Assign the control to the user who will take the action</span></span> |
|<span data-ttu-id="81849-111">comentário</span><span class="sxs-lookup"><span data-stu-id="81849-111">comment</span></span> | <span data-ttu-id="81849-112">string</span><span class="sxs-lookup"><span data-stu-id="81849-112">string</span></span> | <span data-ttu-id="81849-113">Fornece comentários opcionais sobre o controle</span><span class="sxs-lookup"><span data-stu-id="81849-113">Provides optional comment about the control</span></span> |
|<span data-ttu-id="81849-114">estado</span><span class="sxs-lookup"><span data-stu-id="81849-114">state</span></span> | <span data-ttu-id="81849-115">string</span><span class="sxs-lookup"><span data-stu-id="81849-115">string</span></span> | <span data-ttu-id="81849-116">O estado do controle pode ser modificado usando o comando PATCH (ex: ignorado, terceiros etc.)</span><span class="sxs-lookup"><span data-stu-id="81849-116">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
|<span data-ttu-id="81849-117">updatedBy</span><span class="sxs-lookup"><span data-stu-id="81849-117">updatedBy</span></span> | <span data-ttu-id="81849-118">string</span><span class="sxs-lookup"><span data-stu-id="81849-118">string</span></span> |<span data-ttu-id="81849-119">ID do usuário que atualizou o estado do locatário</span><span class="sxs-lookup"><span data-stu-id="81849-119">ID of the user who updated tenant state</span></span> |
|<span data-ttu-id="81849-120">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="81849-120">updatedDateTime</span></span> | <span data-ttu-id="81849-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81849-121">DateTimeOffset</span></span> |<span data-ttu-id="81849-122">Hora em que o estado de controle foi atualizado</span><span class="sxs-lookup"><span data-stu-id="81849-122">Time at which control state was updated</span></span> |
 ## <a name="json-representation"></a><span data-ttu-id="81849-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="81849-123">JSON representation</span></span>
 <span data-ttu-id="81849-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="81849-124">The following is a JSON representation of the resource.</span></span>
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
