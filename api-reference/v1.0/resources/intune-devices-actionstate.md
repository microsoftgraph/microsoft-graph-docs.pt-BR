---
title: tipo de enum actionState
description: Estado da ação no dispositivo
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c0c05e283b94473a5c8c43498ff5bf1dd82da7a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871936"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="52e21-103">tipo de enum actionState</span><span class="sxs-lookup"><span data-stu-id="52e21-103">actionState enum type</span></span>

> <span data-ttu-id="52e21-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="52e21-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="52e21-105">Estado da ação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="52e21-105">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="52e21-106">Membros</span><span class="sxs-lookup"><span data-stu-id="52e21-106">Members</span></span>
|<span data-ttu-id="52e21-107">Membro</span><span class="sxs-lookup"><span data-stu-id="52e21-107">Member</span></span>|<span data-ttu-id="52e21-108">Valor</span><span class="sxs-lookup"><span data-stu-id="52e21-108">Value</span></span>|<span data-ttu-id="52e21-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="52e21-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52e21-110">nenhum</span><span class="sxs-lookup"><span data-stu-id="52e21-110">none</span></span>|<span data-ttu-id="52e21-111">0</span><span class="sxs-lookup"><span data-stu-id="52e21-111">0</span></span>|<span data-ttu-id="52e21-112">Não é um estado de ação válido</span><span class="sxs-lookup"><span data-stu-id="52e21-112">Not a valid action state</span></span>|
|<span data-ttu-id="52e21-113">pendente</span><span class="sxs-lookup"><span data-stu-id="52e21-113">pending</span></span>|<span data-ttu-id="52e21-114">1</span><span class="sxs-lookup"><span data-stu-id="52e21-114">1</span></span>|<span data-ttu-id="52e21-115">A ação é pendente</span><span class="sxs-lookup"><span data-stu-id="52e21-115">Action is pending</span></span>|
|<span data-ttu-id="52e21-116">cancelado</span><span class="sxs-lookup"><span data-stu-id="52e21-116">canceled</span></span>|<span data-ttu-id="52e21-117">2</span><span class="sxs-lookup"><span data-stu-id="52e21-117">2</span></span>|<span data-ttu-id="52e21-118">Ação foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="52e21-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="52e21-119">ativo</span><span class="sxs-lookup"><span data-stu-id="52e21-119">active</span></span>|<span data-ttu-id="52e21-120">3</span><span class="sxs-lookup"><span data-stu-id="52e21-120">3</span></span>|<span data-ttu-id="52e21-121">Ação está ativa.</span><span class="sxs-lookup"><span data-stu-id="52e21-121">Action is active.</span></span>|
|<span data-ttu-id="52e21-122">done</span><span class="sxs-lookup"><span data-stu-id="52e21-122">done</span></span>|<span data-ttu-id="52e21-123">4</span><span class="sxs-lookup"><span data-stu-id="52e21-123">4</span></span>|<span data-ttu-id="52e21-124">Ação concluída sem erros.</span><span class="sxs-lookup"><span data-stu-id="52e21-124">Action completed without errors.</span></span>|
|<span data-ttu-id="52e21-125">Falha</span><span class="sxs-lookup"><span data-stu-id="52e21-125">failed</span></span>|<span data-ttu-id="52e21-126">5</span><span class="sxs-lookup"><span data-stu-id="52e21-126">5</span></span>|<span data-ttu-id="52e21-127">Falha na ação</span><span class="sxs-lookup"><span data-stu-id="52e21-127">Action failed</span></span>|
|<span data-ttu-id="52e21-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="52e21-128">notSupported</span></span>|<span data-ttu-id="52e21-129">6</span><span class="sxs-lookup"><span data-stu-id="52e21-129">6</span></span>|<span data-ttu-id="52e21-130">Não há suporte para a ação.</span><span class="sxs-lookup"><span data-stu-id="52e21-130">Action is not supported.</span></span>|



