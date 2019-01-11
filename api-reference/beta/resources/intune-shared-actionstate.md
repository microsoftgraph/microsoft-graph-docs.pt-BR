---
title: tipo de enum actionState
description: Estado da ação no dispositivo
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: af8bb3869171faee5907b4a3f1921bcb70044aec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829901"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="5a452-103">tipo de enum actionState</span><span class="sxs-lookup"><span data-stu-id="5a452-103">actionState enum type</span></span>

> <span data-ttu-id="5a452-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5a452-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a452-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5a452-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5a452-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5a452-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a452-107">Estado da ação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="5a452-107">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="5a452-108">Membros</span><span class="sxs-lookup"><span data-stu-id="5a452-108">Members</span></span>
|<span data-ttu-id="5a452-109">Membro</span><span class="sxs-lookup"><span data-stu-id="5a452-109">Member</span></span>|<span data-ttu-id="5a452-110">Valor</span><span class="sxs-lookup"><span data-stu-id="5a452-110">Value</span></span>|<span data-ttu-id="5a452-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a452-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a452-112">nenhum</span><span class="sxs-lookup"><span data-stu-id="5a452-112">none</span></span>|<span data-ttu-id="5a452-113">0</span><span class="sxs-lookup"><span data-stu-id="5a452-113">0</span></span>|<span data-ttu-id="5a452-114">Não é um estado de ação válido</span><span class="sxs-lookup"><span data-stu-id="5a452-114">Not a valid action state</span></span>|
|<span data-ttu-id="5a452-115">pendente</span><span class="sxs-lookup"><span data-stu-id="5a452-115">pending</span></span>|<span data-ttu-id="5a452-116">1</span><span class="sxs-lookup"><span data-stu-id="5a452-116">1</span></span>|<span data-ttu-id="5a452-117">A ação é pendente</span><span class="sxs-lookup"><span data-stu-id="5a452-117">Action is pending</span></span>|
|<span data-ttu-id="5a452-118">cancelado</span><span class="sxs-lookup"><span data-stu-id="5a452-118">canceled</span></span>|<span data-ttu-id="5a452-119">2</span><span class="sxs-lookup"><span data-stu-id="5a452-119">2</span></span>|<span data-ttu-id="5a452-120">Ação foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="5a452-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="5a452-121">ativo</span><span class="sxs-lookup"><span data-stu-id="5a452-121">active</span></span>|<span data-ttu-id="5a452-122">3</span><span class="sxs-lookup"><span data-stu-id="5a452-122">3</span></span>|<span data-ttu-id="5a452-123">Ação está ativa.</span><span class="sxs-lookup"><span data-stu-id="5a452-123">Action is active.</span></span>|
|<span data-ttu-id="5a452-124">done</span><span class="sxs-lookup"><span data-stu-id="5a452-124">done</span></span>|<span data-ttu-id="5a452-125">4</span><span class="sxs-lookup"><span data-stu-id="5a452-125">4</span></span>|<span data-ttu-id="5a452-126">Ação concluída sem erros.</span><span class="sxs-lookup"><span data-stu-id="5a452-126">Action completed without errors.</span></span>|
|<span data-ttu-id="5a452-127">Falha</span><span class="sxs-lookup"><span data-stu-id="5a452-127">failed</span></span>|<span data-ttu-id="5a452-128">5</span><span class="sxs-lookup"><span data-stu-id="5a452-128">5</span></span>|<span data-ttu-id="5a452-129">Falha na ação</span><span class="sxs-lookup"><span data-stu-id="5a452-129">Action failed</span></span>|
|<span data-ttu-id="5a452-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="5a452-130">notSupported</span></span>|<span data-ttu-id="5a452-131">6</span><span class="sxs-lookup"><span data-stu-id="5a452-131">6</span></span>|<span data-ttu-id="5a452-132">Não há suporte para a ação.</span><span class="sxs-lookup"><span data-stu-id="5a452-132">Action is not supported.</span></span>|





