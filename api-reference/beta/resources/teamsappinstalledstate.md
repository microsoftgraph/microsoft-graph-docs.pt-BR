---
title: Membros
description: Descreve o status atual da instalação de um teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ca42b56e2c374dbaea1df676e3a84569b192e78c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937170"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="a784a-103">tipo de enum teamsAppInstalledState</span><span class="sxs-lookup"><span data-stu-id="a784a-103">teamsAppInstalledState enum type</span></span>

> <span data-ttu-id="a784a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a784a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a784a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a784a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a784a-106">Descreve o status atual da instalação de um [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="a784a-106">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="a784a-107">Membros</span><span class="sxs-lookup"><span data-stu-id="a784a-107">Members</span></span>

| <span data-ttu-id="a784a-108">Membro</span><span class="sxs-lookup"><span data-stu-id="a784a-108">Member</span></span> | <span data-ttu-id="a784a-109">Valor</span><span class="sxs-lookup"><span data-stu-id="a784a-109">Value</span></span>| <span data-ttu-id="a784a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a784a-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a784a-111">notInstalled</span><span class="sxs-lookup"><span data-stu-id="a784a-111">notInstalled</span></span>|<span data-ttu-id="a784a-112">0</span><span class="sxs-lookup"><span data-stu-id="a784a-112">0</span></span>|<span data-ttu-id="a784a-113">Aplicativo não está instalado para a equipe.</span><span class="sxs-lookup"><span data-stu-id="a784a-113">App is not installed to team.</span></span>|
|<span data-ttu-id="a784a-114">instalado</span><span class="sxs-lookup"><span data-stu-id="a784a-114">installed</span></span>|<span data-ttu-id="a784a-115">1</span><span class="sxs-lookup"><span data-stu-id="a784a-115">1</span></span>|<span data-ttu-id="a784a-116">App é instalado normalmente.</span><span class="sxs-lookup"><span data-stu-id="a784a-116">App is installed normally.</span></span>|
|<span data-ttu-id="a784a-117">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="a784a-117">installedAndHidden</span></span>|<span data-ttu-id="a784a-118">2</span><span class="sxs-lookup"><span data-stu-id="a784a-118">2</span></span>|<span data-ttu-id="a784a-119">App está instalado, mas oculto da exibição.</span><span class="sxs-lookup"><span data-stu-id="a784a-119">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="a784a-120">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="a784a-120">installedAndPermanent</span></span>|<span data-ttu-id="a784a-121">3</span><span class="sxs-lookup"><span data-stu-id="a784a-121">3</span></span>|<span data-ttu-id="a784a-122">App permanentemente é instalado e não pode ser removido.</span><span class="sxs-lookup"><span data-stu-id="a784a-122">App is permanently installed and may not be removed.</span></span>|
