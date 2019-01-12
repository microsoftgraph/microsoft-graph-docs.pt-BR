---
title: tipo de enum actionState
description: Estado da ação no dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 14ec93848deccb7d6bb21331095f9ecf4a881815
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990849"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="b2f12-103">tipo de enum actionState</span><span class="sxs-lookup"><span data-stu-id="b2f12-103">actionState enum type</span></span>

> <span data-ttu-id="b2f12-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b2f12-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2f12-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b2f12-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b2f12-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b2f12-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2f12-107">Estado da ação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="b2f12-107">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="b2f12-108">Membros</span><span class="sxs-lookup"><span data-stu-id="b2f12-108">Members</span></span>
|<span data-ttu-id="b2f12-109">Membro</span><span class="sxs-lookup"><span data-stu-id="b2f12-109">Member</span></span>|<span data-ttu-id="b2f12-110">Valor</span><span class="sxs-lookup"><span data-stu-id="b2f12-110">Value</span></span>|<span data-ttu-id="b2f12-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2f12-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2f12-112">nenhum</span><span class="sxs-lookup"><span data-stu-id="b2f12-112">none</span></span>|<span data-ttu-id="b2f12-113">0</span><span class="sxs-lookup"><span data-stu-id="b2f12-113">0</span></span>|<span data-ttu-id="b2f12-114">Não é um estado de ação válido</span><span class="sxs-lookup"><span data-stu-id="b2f12-114">Not a valid action state</span></span>|
|<span data-ttu-id="b2f12-115">pendente</span><span class="sxs-lookup"><span data-stu-id="b2f12-115">pending</span></span>|<span data-ttu-id="b2f12-116">1</span><span class="sxs-lookup"><span data-stu-id="b2f12-116">1</span></span>|<span data-ttu-id="b2f12-117">A ação é pendente</span><span class="sxs-lookup"><span data-stu-id="b2f12-117">Action is pending</span></span>|
|<span data-ttu-id="b2f12-118">cancelado</span><span class="sxs-lookup"><span data-stu-id="b2f12-118">canceled</span></span>|<span data-ttu-id="b2f12-119">2</span><span class="sxs-lookup"><span data-stu-id="b2f12-119">2</span></span>|<span data-ttu-id="b2f12-120">Ação foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="b2f12-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="b2f12-121">ativo</span><span class="sxs-lookup"><span data-stu-id="b2f12-121">active</span></span>|<span data-ttu-id="b2f12-122">3</span><span class="sxs-lookup"><span data-stu-id="b2f12-122">3</span></span>|<span data-ttu-id="b2f12-123">Ação está ativa.</span><span class="sxs-lookup"><span data-stu-id="b2f12-123">Action is active.</span></span>|
|<span data-ttu-id="b2f12-124">done</span><span class="sxs-lookup"><span data-stu-id="b2f12-124">done</span></span>|<span data-ttu-id="b2f12-125">4</span><span class="sxs-lookup"><span data-stu-id="b2f12-125">4</span></span>|<span data-ttu-id="b2f12-126">Ação concluída sem erros.</span><span class="sxs-lookup"><span data-stu-id="b2f12-126">Action completed without errors.</span></span>|
|<span data-ttu-id="b2f12-127">Falha</span><span class="sxs-lookup"><span data-stu-id="b2f12-127">failed</span></span>|<span data-ttu-id="b2f12-128">5</span><span class="sxs-lookup"><span data-stu-id="b2f12-128">5</span></span>|<span data-ttu-id="b2f12-129">Falha na ação</span><span class="sxs-lookup"><span data-stu-id="b2f12-129">Action failed</span></span>|
|<span data-ttu-id="b2f12-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="b2f12-130">notSupported</span></span>|<span data-ttu-id="b2f12-131">6</span><span class="sxs-lookup"><span data-stu-id="b2f12-131">6</span></span>|<span data-ttu-id="b2f12-132">Não há suporte para a ação.</span><span class="sxs-lookup"><span data-stu-id="b2f12-132">Action is not supported.</span></span>|





