---
title: Membros
description: 'Descreve a visibilidade de uma equipe. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 7e77fbd2667f8656a4c2f66046636ff73ac8891d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521345"
---
# <a name="teamvisibilitytype-enum-type"></a><span data-ttu-id="91649-103">tipo de enum teamVisibilityType</span><span class="sxs-lookup"><span data-stu-id="91649-103">teamVisibilityType enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91649-104">Descreve a visibilidade de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="91649-104">Describes the visibility of a [team](../resources/team.md).</span></span> 

## <a name="members"></a><span data-ttu-id="91649-105">Membros</span><span class="sxs-lookup"><span data-stu-id="91649-105">Members</span></span>

| <span data-ttu-id="91649-106">Membro</span><span class="sxs-lookup"><span data-stu-id="91649-106">Member</span></span> | <span data-ttu-id="91649-107">Valor</span><span class="sxs-lookup"><span data-stu-id="91649-107">Value</span></span>| <span data-ttu-id="91649-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="91649-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="91649-109">Private</span><span class="sxs-lookup"><span data-stu-id="91649-109">private</span></span>|<span data-ttu-id="91649-110">.0</span><span class="sxs-lookup"><span data-stu-id="91649-110">0</span></span>|<span data-ttu-id="91649-111">Qualquer pessoa pode ver a equipe, mas apenas o proprietário pode adicionar um usuário para a equipe.</span><span class="sxs-lookup"><span data-stu-id="91649-111">Anyone can see the team but only the owner can add a user to the team.</span></span>|
|<span data-ttu-id="91649-112">public</span><span class="sxs-lookup"><span data-stu-id="91649-112">public</span></span>|<span data-ttu-id="91649-113">-1</span><span class="sxs-lookup"><span data-stu-id="91649-113">1</span></span>|<span data-ttu-id="91649-114">Qualquer pessoa pode participar da equipe.</span><span class="sxs-lookup"><span data-stu-id="91649-114">Anyone can join the team.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamvisibilitytype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
