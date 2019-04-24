---
title: Membros
description: 'Descreve a visibilidade de uma equipe. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ea8868924681d3e8f8cd0b4f55ff947c085260e0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456963"
---
# <a name="teamvisibilitytype-enum-type"></a><span data-ttu-id="2cf55-103">tipo de enumeração teamVisibilityType</span><span class="sxs-lookup"><span data-stu-id="2cf55-103">teamVisibilityType enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2cf55-104">Descreve a visibilidade de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="2cf55-104">Describes the visibility of a [team](../resources/team.md).</span></span> 

## <a name="members"></a><span data-ttu-id="2cf55-105">Membros</span><span class="sxs-lookup"><span data-stu-id="2cf55-105">Members</span></span>

| <span data-ttu-id="2cf55-106">Membro</span><span class="sxs-lookup"><span data-stu-id="2cf55-106">Member</span></span> | <span data-ttu-id="2cf55-107">Valor</span><span class="sxs-lookup"><span data-stu-id="2cf55-107">Value</span></span>| <span data-ttu-id="2cf55-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cf55-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2cf55-109">privada</span><span class="sxs-lookup"><span data-stu-id="2cf55-109">private</span></span>|<span data-ttu-id="2cf55-110">,0</span><span class="sxs-lookup"><span data-stu-id="2cf55-110">0</span></span>|<span data-ttu-id="2cf55-111">Qualquer pessoa pode ver a equipe, mas apenas o proprietário pode adicionar um usuário à equipe.</span><span class="sxs-lookup"><span data-stu-id="2cf55-111">Anyone can see the team but only the owner can add a user to the team.</span></span>|
|<span data-ttu-id="2cf55-112">public</span><span class="sxs-lookup"><span data-stu-id="2cf55-112">public</span></span>|<span data-ttu-id="2cf55-113">1</span><span class="sxs-lookup"><span data-stu-id="2cf55-113">1</span></span>|<span data-ttu-id="2cf55-114">Qualquer pessoa pode participar da equipe.</span><span class="sxs-lookup"><span data-stu-id="2cf55-114">Anyone can join the team.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamvisibilitytype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
