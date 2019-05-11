---
title: tipo de enumeração vppTokenState
description: Estados possíveis associados a um token do Apple Volume Purchase Program.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fd568bdb4430f61a52577617876a682cc4f7ed99
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940236"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="d83eb-103">tipo de enumeração vppTokenState</span><span class="sxs-lookup"><span data-stu-id="d83eb-103">vppTokenState enum type</span></span>

> <span data-ttu-id="d83eb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d83eb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d83eb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d83eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d83eb-106">Estados possíveis associados a um token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="d83eb-106">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="d83eb-107">Membros</span><span class="sxs-lookup"><span data-stu-id="d83eb-107">Members</span></span>
|<span data-ttu-id="d83eb-108">Membro</span><span class="sxs-lookup"><span data-stu-id="d83eb-108">Member</span></span>|<span data-ttu-id="d83eb-109">Valor</span><span class="sxs-lookup"><span data-stu-id="d83eb-109">Value</span></span>|<span data-ttu-id="d83eb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d83eb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d83eb-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="d83eb-111">unknown</span></span>|<span data-ttu-id="d83eb-112">,0</span><span class="sxs-lookup"><span data-stu-id="d83eb-112">0</span></span>|<span data-ttu-id="d83eb-113">Estado padrão.</span><span class="sxs-lookup"><span data-stu-id="d83eb-113">Default state.</span></span>|
|<span data-ttu-id="d83eb-114">inválido</span><span class="sxs-lookup"><span data-stu-id="d83eb-114">valid</span></span>|<span data-ttu-id="d83eb-115">1</span><span class="sxs-lookup"><span data-stu-id="d83eb-115">1</span></span>|<span data-ttu-id="d83eb-116">O token é válido.</span><span class="sxs-lookup"><span data-stu-id="d83eb-116">Token is valid.</span></span>|
|<span data-ttu-id="d83eb-117">venceu</span><span class="sxs-lookup"><span data-stu-id="d83eb-117">expired</span></span>|<span data-ttu-id="d83eb-118">duas</span><span class="sxs-lookup"><span data-stu-id="d83eb-118">2</span></span>|<span data-ttu-id="d83eb-119">O token expirou.</span><span class="sxs-lookup"><span data-stu-id="d83eb-119">Token is expired.</span></span>|
|<span data-ttu-id="d83eb-120">Inválido</span><span class="sxs-lookup"><span data-stu-id="d83eb-120">invalid</span></span>|<span data-ttu-id="d83eb-121">3D</span><span class="sxs-lookup"><span data-stu-id="d83eb-121">3</span></span>|<span data-ttu-id="d83eb-122">O token é inválido.</span><span class="sxs-lookup"><span data-stu-id="d83eb-122">Token is invalid.</span></span>|
|<span data-ttu-id="d83eb-123">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="d83eb-123">assignedToExternalMDM</span></span>|<span data-ttu-id="d83eb-124">quatro</span><span class="sxs-lookup"><span data-stu-id="d83eb-124">4</span></span>|<span data-ttu-id="d83eb-125">O token é gerenciado por outro serviço MDM.</span><span class="sxs-lookup"><span data-stu-id="d83eb-125">Token is managed by another MDM Service.</span></span>|




