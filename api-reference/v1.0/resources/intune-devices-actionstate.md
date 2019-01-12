---
title: tipo de enum actionState
description: Estado da ação no dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5579d8de986a764cd96e42dff30c007449130b0b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922442"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="a6917-103">tipo de enum actionState</span><span class="sxs-lookup"><span data-stu-id="a6917-103">actionState enum type</span></span>

> <span data-ttu-id="a6917-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a6917-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6917-105">Estado da ação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="a6917-105">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="a6917-106">Membros</span><span class="sxs-lookup"><span data-stu-id="a6917-106">Members</span></span>
|<span data-ttu-id="a6917-107">Membro</span><span class="sxs-lookup"><span data-stu-id="a6917-107">Member</span></span>|<span data-ttu-id="a6917-108">Valor</span><span class="sxs-lookup"><span data-stu-id="a6917-108">Value</span></span>|<span data-ttu-id="a6917-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6917-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6917-110">nenhum</span><span class="sxs-lookup"><span data-stu-id="a6917-110">none</span></span>|<span data-ttu-id="a6917-111">0</span><span class="sxs-lookup"><span data-stu-id="a6917-111">0</span></span>|<span data-ttu-id="a6917-112">Não é um estado de ação válido</span><span class="sxs-lookup"><span data-stu-id="a6917-112">Not a valid action state</span></span>|
|<span data-ttu-id="a6917-113">pendente</span><span class="sxs-lookup"><span data-stu-id="a6917-113">pending</span></span>|<span data-ttu-id="a6917-114">1</span><span class="sxs-lookup"><span data-stu-id="a6917-114">1</span></span>|<span data-ttu-id="a6917-115">A ação é pendente</span><span class="sxs-lookup"><span data-stu-id="a6917-115">Action is pending</span></span>|
|<span data-ttu-id="a6917-116">cancelado</span><span class="sxs-lookup"><span data-stu-id="a6917-116">canceled</span></span>|<span data-ttu-id="a6917-117">2</span><span class="sxs-lookup"><span data-stu-id="a6917-117">2</span></span>|<span data-ttu-id="a6917-118">Ação foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="a6917-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="a6917-119">ativo</span><span class="sxs-lookup"><span data-stu-id="a6917-119">active</span></span>|<span data-ttu-id="a6917-120">3</span><span class="sxs-lookup"><span data-stu-id="a6917-120">3</span></span>|<span data-ttu-id="a6917-121">Ação está ativa.</span><span class="sxs-lookup"><span data-stu-id="a6917-121">Action is active.</span></span>|
|<span data-ttu-id="a6917-122">done</span><span class="sxs-lookup"><span data-stu-id="a6917-122">done</span></span>|<span data-ttu-id="a6917-123">4</span><span class="sxs-lookup"><span data-stu-id="a6917-123">4</span></span>|<span data-ttu-id="a6917-124">Ação concluída sem erros.</span><span class="sxs-lookup"><span data-stu-id="a6917-124">Action completed without errors.</span></span>|
|<span data-ttu-id="a6917-125">Falha</span><span class="sxs-lookup"><span data-stu-id="a6917-125">failed</span></span>|<span data-ttu-id="a6917-126">5</span><span class="sxs-lookup"><span data-stu-id="a6917-126">5</span></span>|<span data-ttu-id="a6917-127">Falha na ação</span><span class="sxs-lookup"><span data-stu-id="a6917-127">Action failed</span></span>|
|<span data-ttu-id="a6917-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="a6917-128">notSupported</span></span>|<span data-ttu-id="a6917-129">6</span><span class="sxs-lookup"><span data-stu-id="a6917-129">6</span></span>|<span data-ttu-id="a6917-130">Não há suporte para a ação.</span><span class="sxs-lookup"><span data-stu-id="a6917-130">Action is not supported.</span></span>|



