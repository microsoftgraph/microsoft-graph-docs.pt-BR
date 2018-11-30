---
title: tipo de enum actionState
description: Estado da ação no dispositivo
ms.openlocfilehash: 1a18eb87cb4c9162777d16dc866de5f5766c87b1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006956"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="5de6d-103">tipo de enum actionState</span><span class="sxs-lookup"><span data-stu-id="5de6d-103">actionState enum type</span></span>

> <span data-ttu-id="5de6d-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5de6d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5de6d-105">Estado da ação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="5de6d-105">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="5de6d-106">Membros</span><span class="sxs-lookup"><span data-stu-id="5de6d-106">Members</span></span>
|<span data-ttu-id="5de6d-107">Membro</span><span class="sxs-lookup"><span data-stu-id="5de6d-107">Member</span></span>|<span data-ttu-id="5de6d-108">Valor</span><span class="sxs-lookup"><span data-stu-id="5de6d-108">Value</span></span>|<span data-ttu-id="5de6d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5de6d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5de6d-110">nenhum</span><span class="sxs-lookup"><span data-stu-id="5de6d-110">none</span></span>|<span data-ttu-id="5de6d-111">0</span><span class="sxs-lookup"><span data-stu-id="5de6d-111">0</span></span>|<span data-ttu-id="5de6d-112">Não é um estado de ação válido</span><span class="sxs-lookup"><span data-stu-id="5de6d-112">Not a valid action state</span></span>|
|<span data-ttu-id="5de6d-113">pendente</span><span class="sxs-lookup"><span data-stu-id="5de6d-113">pending</span></span>|<span data-ttu-id="5de6d-114">1</span><span class="sxs-lookup"><span data-stu-id="5de6d-114">1</span></span>|<span data-ttu-id="5de6d-115">A ação é pendente</span><span class="sxs-lookup"><span data-stu-id="5de6d-115">Action is pending</span></span>|
|<span data-ttu-id="5de6d-116">cancelado</span><span class="sxs-lookup"><span data-stu-id="5de6d-116">canceled</span></span>|<span data-ttu-id="5de6d-117">2</span><span class="sxs-lookup"><span data-stu-id="5de6d-117">2</span></span>|<span data-ttu-id="5de6d-118">Ação foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="5de6d-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="5de6d-119">ativo</span><span class="sxs-lookup"><span data-stu-id="5de6d-119">active</span></span>|<span data-ttu-id="5de6d-120">3</span><span class="sxs-lookup"><span data-stu-id="5de6d-120">3</span></span>|<span data-ttu-id="5de6d-121">Ação está ativa.</span><span class="sxs-lookup"><span data-stu-id="5de6d-121">Action is active.</span></span>|
|<span data-ttu-id="5de6d-122">done</span><span class="sxs-lookup"><span data-stu-id="5de6d-122">done</span></span>|<span data-ttu-id="5de6d-123">4</span><span class="sxs-lookup"><span data-stu-id="5de6d-123">4</span></span>|<span data-ttu-id="5de6d-124">Ação concluída sem erros.</span><span class="sxs-lookup"><span data-stu-id="5de6d-124">Action completed without errors.</span></span>|
|<span data-ttu-id="5de6d-125">Falha</span><span class="sxs-lookup"><span data-stu-id="5de6d-125">failed</span></span>|<span data-ttu-id="5de6d-126">5</span><span class="sxs-lookup"><span data-stu-id="5de6d-126">5</span></span>|<span data-ttu-id="5de6d-127">Falha na ação</span><span class="sxs-lookup"><span data-stu-id="5de6d-127">Action failed</span></span>|
|<span data-ttu-id="5de6d-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="5de6d-128">notSupported</span></span>|<span data-ttu-id="5de6d-129">6</span><span class="sxs-lookup"><span data-stu-id="5de6d-129">6</span></span>|<span data-ttu-id="5de6d-130">Não há suporte para a ação.</span><span class="sxs-lookup"><span data-stu-id="5de6d-130">Action is not supported.</span></span>|



