---
title: Membros
description: Descreve o status atual da instalação de um teamsApp.
ms.openlocfilehash: 7f358a621a25219e78e3a02ce081d07a27395d2c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039002"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="fdcb7-103">tipo de enum teamsAppInstalledState</span><span class="sxs-lookup"><span data-stu-id="fdcb7-103">teamsAppInstalledState enum type</span></span>

> <span data-ttu-id="fdcb7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fdcb7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fdcb7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fdcb7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fdcb7-106">Descreve o status atual da instalação de um [teamsApp](teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="fdcb7-106">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="fdcb7-107">Membros</span><span class="sxs-lookup"><span data-stu-id="fdcb7-107">Members</span></span>

| <span data-ttu-id="fdcb7-108">Membro</span><span class="sxs-lookup"><span data-stu-id="fdcb7-108">Member</span></span> | <span data-ttu-id="fdcb7-109">Valor</span><span class="sxs-lookup"><span data-stu-id="fdcb7-109">Value</span></span>| <span data-ttu-id="fdcb7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdcb7-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="fdcb7-111">notInstalled</span><span class="sxs-lookup"><span data-stu-id="fdcb7-111">notInstalled</span></span>|<span data-ttu-id="fdcb7-112">0</span><span class="sxs-lookup"><span data-stu-id="fdcb7-112">0</span></span>|<span data-ttu-id="fdcb7-113">Aplicativo não está instalado para a equipe.</span><span class="sxs-lookup"><span data-stu-id="fdcb7-113">App is not installed to team.</span></span>|
|<span data-ttu-id="fdcb7-114">instalado</span><span class="sxs-lookup"><span data-stu-id="fdcb7-114">installed</span></span>|<span data-ttu-id="fdcb7-115">1</span><span class="sxs-lookup"><span data-stu-id="fdcb7-115">1</span></span>|<span data-ttu-id="fdcb7-116">App é instalado normalmente.</span><span class="sxs-lookup"><span data-stu-id="fdcb7-116">App is installed normally.</span></span>|
|<span data-ttu-id="fdcb7-117">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="fdcb7-117">installedAndHidden</span></span>|<span data-ttu-id="fdcb7-118">2</span><span class="sxs-lookup"><span data-stu-id="fdcb7-118">2</span></span>|<span data-ttu-id="fdcb7-119">App está instalado, mas oculto da exibição.</span><span class="sxs-lookup"><span data-stu-id="fdcb7-119">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="fdcb7-120">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="fdcb7-120">installedAndPermanent</span></span>|<span data-ttu-id="fdcb7-121">3</span><span class="sxs-lookup"><span data-stu-id="fdcb7-121">3</span></span>|<span data-ttu-id="fdcb7-122">App permanentemente é instalado e não pode ser removido.</span><span class="sxs-lookup"><span data-stu-id="fdcb7-122">App is permanently installed and may not be removed.</span></span>|
