---
title: Membros
description: Descreve o status de instalação atual de um teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a58a0d046ef9c42f197e841ab542bf8dcb5f96f5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462246"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="841e3-103">tipo de enumeração teamsAppInstalledState</span><span class="sxs-lookup"><span data-stu-id="841e3-103">teamsAppInstalledState enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="841e3-104">Descreve o status de instalação atual de um [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="841e3-104">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="841e3-105">Membros</span><span class="sxs-lookup"><span data-stu-id="841e3-105">Members</span></span>

| <span data-ttu-id="841e3-106">Membro</span><span class="sxs-lookup"><span data-stu-id="841e3-106">Member</span></span> | <span data-ttu-id="841e3-107">Valor</span><span class="sxs-lookup"><span data-stu-id="841e3-107">Value</span></span>| <span data-ttu-id="841e3-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="841e3-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="841e3-109">não instalado</span><span class="sxs-lookup"><span data-stu-id="841e3-109">notInstalled</span></span>|<span data-ttu-id="841e3-110">,0</span><span class="sxs-lookup"><span data-stu-id="841e3-110">0</span></span>|<span data-ttu-id="841e3-111">O aplicativo não está instalado na equipe.</span><span class="sxs-lookup"><span data-stu-id="841e3-111">App is not installed to team.</span></span>|
|<span data-ttu-id="841e3-112">instalação</span><span class="sxs-lookup"><span data-stu-id="841e3-112">installed</span></span>|<span data-ttu-id="841e3-113">1</span><span class="sxs-lookup"><span data-stu-id="841e3-113">1</span></span>|<span data-ttu-id="841e3-114">O aplicativo está instalado normalmente.</span><span class="sxs-lookup"><span data-stu-id="841e3-114">App is installed normally.</span></span>|
|<span data-ttu-id="841e3-115">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="841e3-115">installedAndHidden</span></span>|<span data-ttu-id="841e3-116">duas</span><span class="sxs-lookup"><span data-stu-id="841e3-116">2</span></span>|<span data-ttu-id="841e3-117">O aplicativo está instalado, mas oculto no modo de exibição.</span><span class="sxs-lookup"><span data-stu-id="841e3-117">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="841e3-118">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="841e3-118">installedAndPermanent</span></span>|<span data-ttu-id="841e3-119">3D</span><span class="sxs-lookup"><span data-stu-id="841e3-119">3</span></span>|<span data-ttu-id="841e3-120">O aplicativo está instalado permanentemente e não pode ser removido.</span><span class="sxs-lookup"><span data-stu-id="841e3-120">App is permanently installed and may not be removed.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstalledstate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
