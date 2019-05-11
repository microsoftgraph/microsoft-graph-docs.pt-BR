---
title: tipo de enumeração compliancestate
description: Estado de conformidade.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6dc39839754f24ae25044b0aa249d61fe2655d68
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943030"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="8ac18-103">tipo de enumeração compliancestate</span><span class="sxs-lookup"><span data-stu-id="8ac18-103">complianceState enum type</span></span>

> <span data-ttu-id="8ac18-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8ac18-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ac18-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8ac18-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ac18-106">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="8ac18-106">Compliance state.</span></span>

## <a name="members"></a><span data-ttu-id="8ac18-107">Membros</span><span class="sxs-lookup"><span data-stu-id="8ac18-107">Members</span></span>
|<span data-ttu-id="8ac18-108">Membro</span><span class="sxs-lookup"><span data-stu-id="8ac18-108">Member</span></span>|<span data-ttu-id="8ac18-109">Valor</span><span class="sxs-lookup"><span data-stu-id="8ac18-109">Value</span></span>|<span data-ttu-id="8ac18-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ac18-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ac18-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="8ac18-111">unknown</span></span>|<span data-ttu-id="8ac18-112">,0</span><span class="sxs-lookup"><span data-stu-id="8ac18-112">0</span></span>|<span data-ttu-id="8ac18-113">Unknown.</span><span class="sxs-lookup"><span data-stu-id="8ac18-113">Unknown.</span></span>|
|<span data-ttu-id="8ac18-114">com</span><span class="sxs-lookup"><span data-stu-id="8ac18-114">compliant</span></span>|<span data-ttu-id="8ac18-115">1</span><span class="sxs-lookup"><span data-stu-id="8ac18-115">1</span></span>|<span data-ttu-id="8ac18-116">Com.</span><span class="sxs-lookup"><span data-stu-id="8ac18-116">Compliant.</span></span>|
|<span data-ttu-id="8ac18-117">incompatível</span><span class="sxs-lookup"><span data-stu-id="8ac18-117">noncompliant</span></span>|<span data-ttu-id="8ac18-118">duas</span><span class="sxs-lookup"><span data-stu-id="8ac18-118">2</span></span>|<span data-ttu-id="8ac18-119">O dispositivo não está em conformidade e é bloqueado de recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="8ac18-119">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="8ac18-120">apresentar</span><span class="sxs-lookup"><span data-stu-id="8ac18-120">conflict</span></span>|<span data-ttu-id="8ac18-121">3D</span><span class="sxs-lookup"><span data-stu-id="8ac18-121">3</span></span>|<span data-ttu-id="8ac18-122">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="8ac18-122">Conflict with other rules.</span></span>|
|<span data-ttu-id="8ac18-123">erro</span><span class="sxs-lookup"><span data-stu-id="8ac18-123">error</span></span>|<span data-ttu-id="8ac18-124">quatro</span><span class="sxs-lookup"><span data-stu-id="8ac18-124">4</span></span>|<span data-ttu-id="8ac18-125">Erro</span><span class="sxs-lookup"><span data-stu-id="8ac18-125">Error.</span></span>|
|<span data-ttu-id="8ac18-126">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="8ac18-126">inGracePeriod</span></span>|<span data-ttu-id="8ac18-127">254</span><span class="sxs-lookup"><span data-stu-id="8ac18-127">254</span></span>|<span data-ttu-id="8ac18-128">O dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="8ac18-128">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="8ac18-129">configmanager</span><span class="sxs-lookup"><span data-stu-id="8ac18-129">configManager</span></span>|<span data-ttu-id="8ac18-130">255</span><span class="sxs-lookup"><span data-stu-id="8ac18-130">255</span></span>|<span data-ttu-id="8ac18-131">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="8ac18-131">Managed by Config Manager</span></span>|




