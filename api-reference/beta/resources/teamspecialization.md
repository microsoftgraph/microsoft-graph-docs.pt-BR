---
title: tipo de enum teamSpecialization
description: Descreve o caso de uso especial para uma equipe.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9e19c6b2242256f0d1b7a23c89aa07787bfc1913
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522648"
---
# <a name="teamspecialization-enum-type"></a><span data-ttu-id="7d1f8-103">tipo de enum teamSpecialization</span><span class="sxs-lookup"><span data-stu-id="7d1f8-103">teamSpecialization enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d1f8-104">Indica se a [equipe](../resources/team.md) destina-se de um caso de uso específico.</span><span class="sxs-lookup"><span data-stu-id="7d1f8-104">Indicates whether the [team](../resources/team.md) is intended for a particular use case.</span></span> <span data-ttu-id="7d1f8-105">Especialização cada [equipe](../resources/team.md) tem acesso aos comportamentos exclusivos e experiências destinadas ao seu caso de uso.</span><span class="sxs-lookup"><span data-stu-id="7d1f8-105">Each [team](../resources/team.md) specialization has access to unique behaviors and experiences targeted to its use case.</span></span> <span data-ttu-id="7d1f8-106">O padrão é 'Nenhum'.</span><span class="sxs-lookup"><span data-stu-id="7d1f8-106">Default is 'none'.</span></span>

## <a name="members"></a><span data-ttu-id="7d1f8-107">Membros</span><span class="sxs-lookup"><span data-stu-id="7d1f8-107">Members</span></span>

| <span data-ttu-id="7d1f8-108">Membro</span><span class="sxs-lookup"><span data-stu-id="7d1f8-108">Member</span></span>             | <span data-ttu-id="7d1f8-109">Valor</span><span class="sxs-lookup"><span data-stu-id="7d1f8-109">Value</span></span> | <span data-ttu-id="7d1f8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d1f8-110">Description</span></span>                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| <span data-ttu-id="7d1f8-111">none</span><span class="sxs-lookup"><span data-stu-id="7d1f8-111">none</span></span>               | <span data-ttu-id="7d1f8-112">.0</span><span class="sxs-lookup"><span data-stu-id="7d1f8-112">0</span></span>     | <span data-ttu-id="7d1f8-113">Tipo de uma equipe que dá a experiência de equipe padrão padrão.</span><span class="sxs-lookup"><span data-stu-id="7d1f8-113">Default type for a team which gives the standard team experience.</span></span>          |
| <span data-ttu-id="7d1f8-114">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="7d1f8-114">unknownFutureValue</span></span> | <span data-ttu-id="7d1f8-115">-7</span><span class="sxs-lookup"><span data-stu-id="7d1f8-115">7</span></span>     | <span data-ttu-id="7d1f8-116">Sentinel valor reservado como um espaço reservado para expansão futura do enum.</span><span class="sxs-lookup"><span data-stu-id="7d1f8-116">Sentinel value reserved as a placeholder for future expansion of the enum.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamspecialization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
