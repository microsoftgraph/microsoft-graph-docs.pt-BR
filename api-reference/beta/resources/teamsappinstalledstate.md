---
title: Membros
description: Descreve o status de instalação atual de um teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 82e46faccd2a91a82ba4fb7352391f58a42c33a9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554013"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="7b4ae-103">tipo de enumeração teamsAppInstalledState</span><span class="sxs-lookup"><span data-stu-id="7b4ae-103">teamsAppInstalledState enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b4ae-104">Descreve o status de instalação atual de um [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="7b4ae-104">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="7b4ae-105">Membros</span><span class="sxs-lookup"><span data-stu-id="7b4ae-105">Members</span></span>

| <span data-ttu-id="7b4ae-106">Membro</span><span class="sxs-lookup"><span data-stu-id="7b4ae-106">Member</span></span> | <span data-ttu-id="7b4ae-107">Valor</span><span class="sxs-lookup"><span data-stu-id="7b4ae-107">Value</span></span>| <span data-ttu-id="7b4ae-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b4ae-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7b4ae-109">não instalado</span><span class="sxs-lookup"><span data-stu-id="7b4ae-109">notInstalled</span></span>|<span data-ttu-id="7b4ae-110">,0</span><span class="sxs-lookup"><span data-stu-id="7b4ae-110">0</span></span>|<span data-ttu-id="7b4ae-111">O aplicativo não está instalado na equipe.</span><span class="sxs-lookup"><span data-stu-id="7b4ae-111">App is not installed to team.</span></span>|
|<span data-ttu-id="7b4ae-112">instalação</span><span class="sxs-lookup"><span data-stu-id="7b4ae-112">installed</span></span>|<span data-ttu-id="7b4ae-113">1 </span><span class="sxs-lookup"><span data-stu-id="7b4ae-113">1</span></span>|<span data-ttu-id="7b4ae-114">O aplicativo está instalado normalmente.</span><span class="sxs-lookup"><span data-stu-id="7b4ae-114">App is installed normally.</span></span>|
|<span data-ttu-id="7b4ae-115">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="7b4ae-115">installedAndHidden</span></span>|<span data-ttu-id="7b4ae-116">2 </span><span class="sxs-lookup"><span data-stu-id="7b4ae-116">2</span></span>|<span data-ttu-id="7b4ae-117">O aplicativo está instalado, mas oculto no modo de exibição.</span><span class="sxs-lookup"><span data-stu-id="7b4ae-117">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="7b4ae-118">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="7b4ae-118">installedAndPermanent</span></span>|<span data-ttu-id="7b4ae-119">3 </span><span class="sxs-lookup"><span data-stu-id="7b4ae-119">3</span></span>|<span data-ttu-id="7b4ae-120">O aplicativo está instalado permanentemente e não pode ser removido.</span><span class="sxs-lookup"><span data-stu-id="7b4ae-120">App is permanently installed and may not be removed.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstalledstate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
