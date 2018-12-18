---
title: tipo de enum actionState
description: Estado da ação no dispositivo
author: tfitzmac
ms.openlocfilehash: 1f36c3a6709ade5860ff24cc8d10c2cb0294a471
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315103"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="fceac-103">tipo de enum actionState</span><span class="sxs-lookup"><span data-stu-id="fceac-103">actionState enum type</span></span>

> <span data-ttu-id="fceac-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fceac-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fceac-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fceac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fceac-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fceac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fceac-107">Estado da ação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="fceac-107">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="fceac-108">Membros</span><span class="sxs-lookup"><span data-stu-id="fceac-108">Members</span></span>
|<span data-ttu-id="fceac-109">Membro</span><span class="sxs-lookup"><span data-stu-id="fceac-109">Member</span></span>|<span data-ttu-id="fceac-110">Valor</span><span class="sxs-lookup"><span data-stu-id="fceac-110">Value</span></span>|<span data-ttu-id="fceac-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="fceac-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fceac-112">none</span><span class="sxs-lookup"><span data-stu-id="fceac-112">none</span></span>|<span data-ttu-id="fceac-113">0</span><span class="sxs-lookup"><span data-stu-id="fceac-113">0</span></span>|<span data-ttu-id="fceac-114">Não é um estado de ação válido</span><span class="sxs-lookup"><span data-stu-id="fceac-114">Not a valid action state</span></span>|
|<span data-ttu-id="fceac-115">pendente</span><span class="sxs-lookup"><span data-stu-id="fceac-115">pending</span></span>|<span data-ttu-id="fceac-116">1</span><span class="sxs-lookup"><span data-stu-id="fceac-116">1</span></span>|<span data-ttu-id="fceac-117">A ação é pendente</span><span class="sxs-lookup"><span data-stu-id="fceac-117">Action is pending</span></span>|
|<span data-ttu-id="fceac-118">cancelado</span><span class="sxs-lookup"><span data-stu-id="fceac-118">canceled</span></span>|<span data-ttu-id="fceac-119">2</span><span class="sxs-lookup"><span data-stu-id="fceac-119">2</span></span>|<span data-ttu-id="fceac-120">Ação foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="fceac-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="fceac-121">ativo</span><span class="sxs-lookup"><span data-stu-id="fceac-121">active</span></span>|<span data-ttu-id="fceac-122">3</span><span class="sxs-lookup"><span data-stu-id="fceac-122">3</span></span>|<span data-ttu-id="fceac-123">Ação está ativa.</span><span class="sxs-lookup"><span data-stu-id="fceac-123">Action is active.</span></span>|
|<span data-ttu-id="fceac-124">done</span><span class="sxs-lookup"><span data-stu-id="fceac-124">done</span></span>|<span data-ttu-id="fceac-125">4</span><span class="sxs-lookup"><span data-stu-id="fceac-125">4</span></span>|<span data-ttu-id="fceac-126">Ação concluída sem erros.</span><span class="sxs-lookup"><span data-stu-id="fceac-126">Action completed without errors.</span></span>|
|<span data-ttu-id="fceac-127">Falha</span><span class="sxs-lookup"><span data-stu-id="fceac-127">failed</span></span>|<span data-ttu-id="fceac-128">5</span><span class="sxs-lookup"><span data-stu-id="fceac-128">5</span></span>|<span data-ttu-id="fceac-129">Falha na ação</span><span class="sxs-lookup"><span data-stu-id="fceac-129">Action failed</span></span>|
|<span data-ttu-id="fceac-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="fceac-130">notSupported</span></span>|<span data-ttu-id="fceac-131">6</span><span class="sxs-lookup"><span data-stu-id="fceac-131">6</span></span>|<span data-ttu-id="fceac-132">Não há suporte para a ação.</span><span class="sxs-lookup"><span data-stu-id="fceac-132">Action is not supported.</span></span>|





