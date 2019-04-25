---
title: " tipo de recurso secureScoreControlStateUpdate"
description: Este recurso contém o histórico de Estados de controle atualizados pelo usuário (os Estados de controle incluem Default, ignorado, terceiros).
localization_priority: Normal
ms.openlocfilehash: 8d8c3122a6263ebc7b10b5edfb823953e2d587fc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549136"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="ce512-103">tipo de recurso secureScoreControlStateUpdate</span><span class="sxs-lookup"><span data-stu-id="ce512-103">secureScoreControlStateUpdate resource type</span></span>
<span data-ttu-id="ce512-104">Contém o histórico dos Estados de controle atualizados pelo usuário (os Estados de controle incluem padrão, ignorado, terceiros, reVisado).</span><span class="sxs-lookup"><span data-stu-id="ce512-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="ce512-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce512-105">Property</span></span> |<span data-ttu-id="ce512-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce512-106">Type</span></span> |<span data-ttu-id="ce512-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce512-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="ce512-108">assignedTo</span><span class="sxs-lookup"><span data-stu-id="ce512-108">assignedTo</span></span> | <span data-ttu-id="ce512-109">string</span><span class="sxs-lookup"><span data-stu-id="ce512-109">string</span></span> | <span data-ttu-id="ce512-110">Atribuir o controle ao usuário que executará a ação</span><span class="sxs-lookup"><span data-stu-id="ce512-110">Assign the control to the user who will take the action</span></span> |
|<span data-ttu-id="ce512-111">comentário</span><span class="sxs-lookup"><span data-stu-id="ce512-111">comment</span></span> | <span data-ttu-id="ce512-112">string</span><span class="sxs-lookup"><span data-stu-id="ce512-112">string</span></span> | <span data-ttu-id="ce512-113">Fornece comentários opcionais sobre o controle</span><span class="sxs-lookup"><span data-stu-id="ce512-113">Provides optional comment about the control</span></span> |
|<span data-ttu-id="ce512-114">estado</span><span class="sxs-lookup"><span data-stu-id="ce512-114">state</span></span> | <span data-ttu-id="ce512-115">string</span><span class="sxs-lookup"><span data-stu-id="ce512-115">string</span></span> | <span data-ttu-id="ce512-116">O estado do controle pode ser modificado usando o comando PATCH (ex: ignorado, terceiros etc.)</span><span class="sxs-lookup"><span data-stu-id="ce512-116">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
|<span data-ttu-id="ce512-117">updatedBy</span><span class="sxs-lookup"><span data-stu-id="ce512-117">updatedBy</span></span> | <span data-ttu-id="ce512-118">string</span><span class="sxs-lookup"><span data-stu-id="ce512-118">string</span></span> |<span data-ttu-id="ce512-119">ID do usuário que atualizou o estado do locatário</span><span class="sxs-lookup"><span data-stu-id="ce512-119">ID of the user who updated tenant state</span></span> |
|<span data-ttu-id="ce512-120">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce512-120">updatedDateTime</span></span> | <span data-ttu-id="ce512-121">DateTimeOffset?</span><span class="sxs-lookup"><span data-stu-id="ce512-121">DateTimeOffset?</span></span> |<span data-ttu-id="ce512-122">Hora em que o estado de controle foi atualizado</span><span class="sxs-lookup"><span data-stu-id="ce512-122">Time at which control state was updated</span></span> |
 ## <a name="json-representation"></a><span data-ttu-id="ce512-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ce512-123">JSON representation</span></span>
 <span data-ttu-id="ce512-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ce512-124">The following is a JSON representation of the resource.</span></span>
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
