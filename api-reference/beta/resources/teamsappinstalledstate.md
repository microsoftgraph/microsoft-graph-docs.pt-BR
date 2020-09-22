---
title: Members
description: Descreve o status de instalação atual de um teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 76cecb2b0daa172fd442b0860b71ca94f12e7c7a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046508"
---
# <a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="b823c-103">tipo de enumeração teamsAppInstalledState</span><span class="sxs-lookup"><span data-stu-id="b823c-103">teamsAppInstalledState enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b823c-104">Descreve o status de instalação atual de um [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="b823c-104">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="b823c-105">Membros</span><span class="sxs-lookup"><span data-stu-id="b823c-105">Members</span></span>

| <span data-ttu-id="b823c-106">Membro</span><span class="sxs-lookup"><span data-stu-id="b823c-106">Member</span></span> | <span data-ttu-id="b823c-107">Valor</span><span class="sxs-lookup"><span data-stu-id="b823c-107">Value</span></span>| <span data-ttu-id="b823c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b823c-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b823c-109">não instalado</span><span class="sxs-lookup"><span data-stu-id="b823c-109">notInstalled</span></span>|<span data-ttu-id="b823c-110">,0</span><span class="sxs-lookup"><span data-stu-id="b823c-110">0</span></span>|<span data-ttu-id="b823c-111">O aplicativo não está instalado na equipe.</span><span class="sxs-lookup"><span data-stu-id="b823c-111">App is not installed to team.</span></span>|
|<span data-ttu-id="b823c-112">instalação</span><span class="sxs-lookup"><span data-stu-id="b823c-112">installed</span></span>|<span data-ttu-id="b823c-113">1 </span><span class="sxs-lookup"><span data-stu-id="b823c-113">1</span></span>|<span data-ttu-id="b823c-114">O aplicativo está instalado normalmente.</span><span class="sxs-lookup"><span data-stu-id="b823c-114">App is installed normally.</span></span>|
|<span data-ttu-id="b823c-115">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="b823c-115">installedAndHidden</span></span>|<span data-ttu-id="b823c-116">2 </span><span class="sxs-lookup"><span data-stu-id="b823c-116">2</span></span>|<span data-ttu-id="b823c-117">O aplicativo está instalado, mas oculto no modo de exibição.</span><span class="sxs-lookup"><span data-stu-id="b823c-117">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="b823c-118">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="b823c-118">installedAndPermanent</span></span>|<span data-ttu-id="b823c-119">3 </span><span class="sxs-lookup"><span data-stu-id="b823c-119">3</span></span>|<span data-ttu-id="b823c-120">O aplicativo está instalado permanentemente e não pode ser removido.</span><span class="sxs-lookup"><span data-stu-id="b823c-120">App is permanently installed and may not be removed.</span></span>|


