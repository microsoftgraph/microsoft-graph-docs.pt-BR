---
title: tipo de Enumeração ActionState
description: Estado da ação no dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9e6be5ce422664d5666fd5c76c3ce51ad8a9d798
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027514"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="d28d8-103">tipo de Enumeração ActionState</span><span class="sxs-lookup"><span data-stu-id="d28d8-103">actionState enum type</span></span>

> <span data-ttu-id="d28d8-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d28d8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d28d8-105">Estado da ação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="d28d8-105">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="d28d8-106">Membros</span><span class="sxs-lookup"><span data-stu-id="d28d8-106">Members</span></span>
|<span data-ttu-id="d28d8-107">Membro</span><span class="sxs-lookup"><span data-stu-id="d28d8-107">Member</span></span>|<span data-ttu-id="d28d8-108">Valor</span><span class="sxs-lookup"><span data-stu-id="d28d8-108">Value</span></span>|<span data-ttu-id="d28d8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d28d8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d28d8-110">none</span><span class="sxs-lookup"><span data-stu-id="d28d8-110">none</span></span>|<span data-ttu-id="d28d8-111">,0</span><span class="sxs-lookup"><span data-stu-id="d28d8-111">0</span></span>|<span data-ttu-id="d28d8-112">Não é um estado de ação válido</span><span class="sxs-lookup"><span data-stu-id="d28d8-112">Not a valid action state</span></span>|
|<span data-ttu-id="d28d8-113">função</span><span class="sxs-lookup"><span data-stu-id="d28d8-113">pending</span></span>|<span data-ttu-id="d28d8-114">1</span><span class="sxs-lookup"><span data-stu-id="d28d8-114">1</span></span>|<span data-ttu-id="d28d8-115">Ação pendente</span><span class="sxs-lookup"><span data-stu-id="d28d8-115">Action is pending</span></span>|
|<span data-ttu-id="d28d8-116">foi</span><span class="sxs-lookup"><span data-stu-id="d28d8-116">canceled</span></span>|<span data-ttu-id="d28d8-117">duas</span><span class="sxs-lookup"><span data-stu-id="d28d8-117">2</span></span>|<span data-ttu-id="d28d8-118">A ação foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="d28d8-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="d28d8-119">active</span><span class="sxs-lookup"><span data-stu-id="d28d8-119">active</span></span>|<span data-ttu-id="d28d8-120">3D</span><span class="sxs-lookup"><span data-stu-id="d28d8-120">3</span></span>|<span data-ttu-id="d28d8-121">A ação está ativa.</span><span class="sxs-lookup"><span data-stu-id="d28d8-121">Action is active.</span></span>|
|<span data-ttu-id="d28d8-122">done</span><span class="sxs-lookup"><span data-stu-id="d28d8-122">done</span></span>|<span data-ttu-id="d28d8-123">quatro</span><span class="sxs-lookup"><span data-stu-id="d28d8-123">4</span></span>|<span data-ttu-id="d28d8-124">Ação concluída sem erros.</span><span class="sxs-lookup"><span data-stu-id="d28d8-124">Action completed without errors.</span></span>|
|<span data-ttu-id="d28d8-125">falhou</span><span class="sxs-lookup"><span data-stu-id="d28d8-125">failed</span></span>|<span data-ttu-id="d28d8-126">0,5</span><span class="sxs-lookup"><span data-stu-id="d28d8-126">5</span></span>|<span data-ttu-id="d28d8-127">Falha na ação</span><span class="sxs-lookup"><span data-stu-id="d28d8-127">Action failed</span></span>|
|<span data-ttu-id="d28d8-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="d28d8-128">notSupported</span></span>|<span data-ttu-id="d28d8-129">6</span><span class="sxs-lookup"><span data-stu-id="d28d8-129">6</span></span>|<span data-ttu-id="d28d8-130">Não há suporte para a ação.</span><span class="sxs-lookup"><span data-stu-id="d28d8-130">Action is not supported.</span></span>|



