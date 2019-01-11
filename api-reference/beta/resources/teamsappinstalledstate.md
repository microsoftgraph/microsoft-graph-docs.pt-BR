---
title: Membros
description: Descreve o status atual da instalação de um teamsApp.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 4e453a28b0c3ebc2957cf7e1a92a846e8e4758e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847569"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="d9ed4-103">tipo de enum teamsAppInstalledState</span><span class="sxs-lookup"><span data-stu-id="d9ed4-103">teamsAppInstalledState enum type</span></span>

> <span data-ttu-id="d9ed4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d9ed4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9ed4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d9ed4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d9ed4-106">Descreve o status atual da instalação de um [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="d9ed4-106">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="d9ed4-107">Membros</span><span class="sxs-lookup"><span data-stu-id="d9ed4-107">Members</span></span>

| <span data-ttu-id="d9ed4-108">Membro</span><span class="sxs-lookup"><span data-stu-id="d9ed4-108">Member</span></span> | <span data-ttu-id="d9ed4-109">Valor</span><span class="sxs-lookup"><span data-stu-id="d9ed4-109">Value</span></span>| <span data-ttu-id="d9ed4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9ed4-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d9ed4-111">notInstalled</span><span class="sxs-lookup"><span data-stu-id="d9ed4-111">notInstalled</span></span>|<span data-ttu-id="d9ed4-112">0</span><span class="sxs-lookup"><span data-stu-id="d9ed4-112">0</span></span>|<span data-ttu-id="d9ed4-113">Aplicativo não está instalado para a equipe.</span><span class="sxs-lookup"><span data-stu-id="d9ed4-113">App is not installed to team.</span></span>|
|<span data-ttu-id="d9ed4-114">instalado</span><span class="sxs-lookup"><span data-stu-id="d9ed4-114">installed</span></span>|<span data-ttu-id="d9ed4-115">1</span><span class="sxs-lookup"><span data-stu-id="d9ed4-115">1</span></span>|<span data-ttu-id="d9ed4-116">App é instalado normalmente.</span><span class="sxs-lookup"><span data-stu-id="d9ed4-116">App is installed normally.</span></span>|
|<span data-ttu-id="d9ed4-117">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="d9ed4-117">installedAndHidden</span></span>|<span data-ttu-id="d9ed4-118">2</span><span class="sxs-lookup"><span data-stu-id="d9ed4-118">2</span></span>|<span data-ttu-id="d9ed4-119">App está instalado, mas oculto da exibição.</span><span class="sxs-lookup"><span data-stu-id="d9ed4-119">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="d9ed4-120">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="d9ed4-120">installedAndPermanent</span></span>|<span data-ttu-id="d9ed4-121">3</span><span class="sxs-lookup"><span data-stu-id="d9ed4-121">3</span></span>|<span data-ttu-id="d9ed4-122">App permanentemente é instalado e não pode ser removido.</span><span class="sxs-lookup"><span data-stu-id="d9ed4-122">App is permanently installed and may not be removed.</span></span>|
