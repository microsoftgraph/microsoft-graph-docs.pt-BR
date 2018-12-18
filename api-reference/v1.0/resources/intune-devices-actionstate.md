---
title: tipo de enum actionState
description: Estado da ação no dispositivo
author: tfitzmac
ms.openlocfilehash: 53ee72430ac646bf978a3167b87feaf398c8ac37
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333380"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="f5ec6-103">tipo de enum actionState</span><span class="sxs-lookup"><span data-stu-id="f5ec6-103">actionState enum type</span></span>

> <span data-ttu-id="f5ec6-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f5ec6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5ec6-105">Estado da ação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="f5ec6-105">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="f5ec6-106">Membros</span><span class="sxs-lookup"><span data-stu-id="f5ec6-106">Members</span></span>
|<span data-ttu-id="f5ec6-107">Membro</span><span class="sxs-lookup"><span data-stu-id="f5ec6-107">Member</span></span>|<span data-ttu-id="f5ec6-108">Valor</span><span class="sxs-lookup"><span data-stu-id="f5ec6-108">Value</span></span>|<span data-ttu-id="f5ec6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5ec6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5ec6-110">none</span><span class="sxs-lookup"><span data-stu-id="f5ec6-110">none</span></span>|<span data-ttu-id="f5ec6-111">0</span><span class="sxs-lookup"><span data-stu-id="f5ec6-111">0</span></span>|<span data-ttu-id="f5ec6-112">Não é um estado de ação válido</span><span class="sxs-lookup"><span data-stu-id="f5ec6-112">Not a valid action state</span></span>|
|<span data-ttu-id="f5ec6-113">pendente</span><span class="sxs-lookup"><span data-stu-id="f5ec6-113">pending</span></span>|<span data-ttu-id="f5ec6-114">1</span><span class="sxs-lookup"><span data-stu-id="f5ec6-114">1</span></span>|<span data-ttu-id="f5ec6-115">A ação é pendente</span><span class="sxs-lookup"><span data-stu-id="f5ec6-115">Action is pending</span></span>|
|<span data-ttu-id="f5ec6-116">cancelado</span><span class="sxs-lookup"><span data-stu-id="f5ec6-116">canceled</span></span>|<span data-ttu-id="f5ec6-117">2</span><span class="sxs-lookup"><span data-stu-id="f5ec6-117">2</span></span>|<span data-ttu-id="f5ec6-118">Ação foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="f5ec6-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="f5ec6-119">ativo</span><span class="sxs-lookup"><span data-stu-id="f5ec6-119">active</span></span>|<span data-ttu-id="f5ec6-120">3</span><span class="sxs-lookup"><span data-stu-id="f5ec6-120">3</span></span>|<span data-ttu-id="f5ec6-121">Ação está ativa.</span><span class="sxs-lookup"><span data-stu-id="f5ec6-121">Action is active.</span></span>|
|<span data-ttu-id="f5ec6-122">done</span><span class="sxs-lookup"><span data-stu-id="f5ec6-122">done</span></span>|<span data-ttu-id="f5ec6-123">4</span><span class="sxs-lookup"><span data-stu-id="f5ec6-123">4</span></span>|<span data-ttu-id="f5ec6-124">Ação concluída sem erros.</span><span class="sxs-lookup"><span data-stu-id="f5ec6-124">Action completed without errors.</span></span>|
|<span data-ttu-id="f5ec6-125">Falha</span><span class="sxs-lookup"><span data-stu-id="f5ec6-125">failed</span></span>|<span data-ttu-id="f5ec6-126">5</span><span class="sxs-lookup"><span data-stu-id="f5ec6-126">5</span></span>|<span data-ttu-id="f5ec6-127">Falha na ação</span><span class="sxs-lookup"><span data-stu-id="f5ec6-127">Action failed</span></span>|
|<span data-ttu-id="f5ec6-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="f5ec6-128">notSupported</span></span>|<span data-ttu-id="f5ec6-129">6</span><span class="sxs-lookup"><span data-stu-id="f5ec6-129">6</span></span>|<span data-ttu-id="f5ec6-130">Não há suporte para a ação.</span><span class="sxs-lookup"><span data-stu-id="f5ec6-130">Action is not supported.</span></span>|



