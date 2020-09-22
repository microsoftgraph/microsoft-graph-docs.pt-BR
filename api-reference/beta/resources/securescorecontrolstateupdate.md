---
title: " tipo de recurso secureScoreControlStateUpdate"
description: Este recurso contém o histórico de Estados de controle atualizados pelo usuário (os Estados de controle incluem Default, ignorado, terceiros).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: d1678d4fe77ade738f7eb298221772ced381e2d1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087548"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a><span data-ttu-id="d4a19-103">tipo de recurso secureScoreControlStateUpdate</span><span class="sxs-lookup"><span data-stu-id="d4a19-103">secureScoreControlStateUpdate resource type</span></span>
<span data-ttu-id="d4a19-104">Contém o histórico dos Estados de controle atualizados pelo usuário (os Estados de controle incluem padrão, ignorado, terceiros, revisado).</span><span class="sxs-lookup"><span data-stu-id="d4a19-104">Contains the history of the control states updated by the user (control states include Default, Ignored, ThirdParty, Reviewed).</span></span>

|<span data-ttu-id="d4a19-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d4a19-105">Property</span></span> |<span data-ttu-id="d4a19-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4a19-106">Type</span></span> |<span data-ttu-id="d4a19-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4a19-107">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="d4a19-108">assignedTo</span><span class="sxs-lookup"><span data-stu-id="d4a19-108">assignedTo</span></span> | <span data-ttu-id="d4a19-109">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4a19-109">string</span></span> | <span data-ttu-id="d4a19-110">Atribuir o controle ao usuário que executará a ação</span><span class="sxs-lookup"><span data-stu-id="d4a19-110">Assign the control to the user who will take the action</span></span> |
|<span data-ttu-id="d4a19-111">comment</span><span class="sxs-lookup"><span data-stu-id="d4a19-111">comment</span></span> | <span data-ttu-id="d4a19-112">string</span><span class="sxs-lookup"><span data-stu-id="d4a19-112">string</span></span> | <span data-ttu-id="d4a19-113">Fornece comentários opcionais sobre o controle</span><span class="sxs-lookup"><span data-stu-id="d4a19-113">Provides optional comment about the control</span></span> |
|<span data-ttu-id="d4a19-114">estado</span><span class="sxs-lookup"><span data-stu-id="d4a19-114">state</span></span> | <span data-ttu-id="d4a19-115">string</span><span class="sxs-lookup"><span data-stu-id="d4a19-115">string</span></span> | <span data-ttu-id="d4a19-116">O estado do controle pode ser modificado usando o comando PATCH (ex: ignorado, terceiros etc.)</span><span class="sxs-lookup"><span data-stu-id="d4a19-116">State of the control can be modified using PATCH command(Ex: ignored, thirdParty etc)</span></span> |
|<span data-ttu-id="d4a19-117">updatedBy</span><span class="sxs-lookup"><span data-stu-id="d4a19-117">updatedBy</span></span> | <span data-ttu-id="d4a19-118">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d4a19-118">string</span></span> |<span data-ttu-id="d4a19-119">ID do usuário que atualizou o estado do locatário</span><span class="sxs-lookup"><span data-stu-id="d4a19-119">ID of the user who updated tenant state</span></span> |
|<span data-ttu-id="d4a19-120">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4a19-120">updatedDateTime</span></span> | <span data-ttu-id="d4a19-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4a19-121">DateTimeOffset</span></span> |<span data-ttu-id="d4a19-122">Hora em que o estado de controle foi atualizado</span><span class="sxs-lookup"><span data-stu-id="d4a19-122">Time at which control state was updated</span></span> |
 ## <a name="json-representation"></a><span data-ttu-id="d4a19-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d4a19-123">JSON representation</span></span>
 <span data-ttu-id="d4a19-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d4a19-124">The following is a JSON representation of the resource.</span></span>
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


