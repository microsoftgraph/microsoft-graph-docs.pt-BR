---
title: Membros
description: Descreve o status atual da instalação de um teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 82e46faccd2a91a82ba4fb7352391f58a42c33a9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517271"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="fc0c0-103">tipo de enum teamsAppInstalledState</span><span class="sxs-lookup"><span data-stu-id="fc0c0-103">teamsAppInstalledState enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc0c0-104">Descreve o status atual da instalação de um [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="fc0c0-104">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="fc0c0-105">Membros</span><span class="sxs-lookup"><span data-stu-id="fc0c0-105">Members</span></span>

| <span data-ttu-id="fc0c0-106">Membro</span><span class="sxs-lookup"><span data-stu-id="fc0c0-106">Member</span></span> | <span data-ttu-id="fc0c0-107">Valor</span><span class="sxs-lookup"><span data-stu-id="fc0c0-107">Value</span></span>| <span data-ttu-id="fc0c0-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc0c0-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="fc0c0-109">notInstalled</span><span class="sxs-lookup"><span data-stu-id="fc0c0-109">notInstalled</span></span>|<span data-ttu-id="fc0c0-110">.0</span><span class="sxs-lookup"><span data-stu-id="fc0c0-110">0</span></span>|<span data-ttu-id="fc0c0-111">Aplicativo não está instalado para a equipe.</span><span class="sxs-lookup"><span data-stu-id="fc0c0-111">App is not installed to team.</span></span>|
|<span data-ttu-id="fc0c0-112">Installed</span><span class="sxs-lookup"><span data-stu-id="fc0c0-112">installed</span></span>|<span data-ttu-id="fc0c0-113">-1</span><span class="sxs-lookup"><span data-stu-id="fc0c0-113">1</span></span>|<span data-ttu-id="fc0c0-114">App é instalado normalmente.</span><span class="sxs-lookup"><span data-stu-id="fc0c0-114">App is installed normally.</span></span>|
|<span data-ttu-id="fc0c0-115">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="fc0c0-115">installedAndHidden</span></span>|<span data-ttu-id="fc0c0-116">-2</span><span class="sxs-lookup"><span data-stu-id="fc0c0-116">2</span></span>|<span data-ttu-id="fc0c0-117">App está instalado, mas oculto da exibição.</span><span class="sxs-lookup"><span data-stu-id="fc0c0-117">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="fc0c0-118">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="fc0c0-118">installedAndPermanent</span></span>|<span data-ttu-id="fc0c0-119">-3</span><span class="sxs-lookup"><span data-stu-id="fc0c0-119">3</span></span>|<span data-ttu-id="fc0c0-120">App permanentemente é instalado e não pode ser removido.</span><span class="sxs-lookup"><span data-stu-id="fc0c0-120">App is permanently installed and may not be removed.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstalledstate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
