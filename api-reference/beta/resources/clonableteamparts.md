---
title: tipo de enum clonableTeamParts
description: 'Descreve qual parte de uma equipe deve ser fechado. '
localization_priority: Normal
ms.openlocfilehash: 3169d6e367484248e581c12c38887e07cf5c95af
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511461"
---
# <a name="clonableteamparts-enum-type"></a><span data-ttu-id="ff572-103">tipo de enum clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="ff572-103">clonableTeamParts enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff572-104">Descreve qual parte de uma [equipe](../resources/team.md) deve ser fechado.</span><span class="sxs-lookup"><span data-stu-id="ff572-104">Describes which part of a [team](../resources/team.md) should be cloned.</span></span> 

## <a name="members"></a><span data-ttu-id="ff572-105">Membros</span><span class="sxs-lookup"><span data-stu-id="ff572-105">Members</span></span>

| <span data-ttu-id="ff572-106">Membro</span><span class="sxs-lookup"><span data-stu-id="ff572-106">Member</span></span> | <span data-ttu-id="ff572-107">Valor</span><span class="sxs-lookup"><span data-stu-id="ff572-107">Value</span></span>| <span data-ttu-id="ff572-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff572-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ff572-109">Aplicativos</span><span class="sxs-lookup"><span data-stu-id="ff572-109">apps</span></span>|<span data-ttu-id="ff572-110">-1</span><span class="sxs-lookup"><span data-stu-id="ff572-110">1</span></span>|<span data-ttu-id="ff572-111">Copie a lista de aplicativos instalados.</span><span class="sxs-lookup"><span data-stu-id="ff572-111">Copy the list of installed apps.</span></span>|
|<span data-ttu-id="ff572-112">guias</span><span class="sxs-lookup"><span data-stu-id="ff572-112">tabs</span></span>|<span data-ttu-id="ff572-113">-2</span><span class="sxs-lookup"><span data-stu-id="ff572-113">2</span></span>|<span data-ttu-id="ff572-114">copia as guias no canais.</span><span class="sxs-lookup"><span data-stu-id="ff572-114">copies the tabs within channels.</span></span>|
|<span data-ttu-id="ff572-115">configurações</span><span class="sxs-lookup"><span data-stu-id="ff572-115">settings</span></span>|<span data-ttu-id="ff572-116">4\*</span><span class="sxs-lookup"><span data-stu-id="ff572-116">4</span></span>|<span data-ttu-id="ff572-117">Copia todas as definições dentro da equipe, juntamente com as configurações de chave de grupo.</span><span class="sxs-lookup"><span data-stu-id="ff572-117">Copies all settings within the team, along with key group settings.</span></span>|
|<span data-ttu-id="ff572-118">canais</span><span class="sxs-lookup"><span data-stu-id="ff572-118">channels</span></span>|<span data-ttu-id="ff572-119">8\*</span><span class="sxs-lookup"><span data-stu-id="ff572-119">8</span></span>|<span data-ttu-id="ff572-120">Copia a estrutura de canal (mas não as mensagens no canal).</span><span class="sxs-lookup"><span data-stu-id="ff572-120">copies the channel structure (but not the messages in the channel).</span></span>|
|<span data-ttu-id="ff572-121">membros</span><span class="sxs-lookup"><span data-stu-id="ff572-121">members</span></span>|<span data-ttu-id="ff572-122">16\*\*</span><span class="sxs-lookup"><span data-stu-id="ff572-122">16</span></span>|<span data-ttu-id="ff572-123">copia os membros e proprietários da equipe.</span><span class="sxs-lookup"><span data-stu-id="ff572-123">copies the members and owners of the team.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/clonableteamparts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
