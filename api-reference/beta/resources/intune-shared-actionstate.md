---
title: tipo de enum actionState
description: Estado da ação no dispositivo
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 54f9a636cb579a234097f86aba8cf4e8fb8fefd0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421610"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="99bcf-103">tipo de enum actionState</span><span class="sxs-lookup"><span data-stu-id="99bcf-103">actionState enum type</span></span>

> <span data-ttu-id="99bcf-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="99bcf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="99bcf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="99bcf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="99bcf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="99bcf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99bcf-107">Estado da ação no dispositivo</span><span class="sxs-lookup"><span data-stu-id="99bcf-107">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="99bcf-108">Membros</span><span class="sxs-lookup"><span data-stu-id="99bcf-108">Members</span></span>
|<span data-ttu-id="99bcf-109">Membro</span><span class="sxs-lookup"><span data-stu-id="99bcf-109">Member</span></span>|<span data-ttu-id="99bcf-110">Valor</span><span class="sxs-lookup"><span data-stu-id="99bcf-110">Value</span></span>|<span data-ttu-id="99bcf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="99bcf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99bcf-112">none</span><span class="sxs-lookup"><span data-stu-id="99bcf-112">none</span></span>|<span data-ttu-id="99bcf-113">0</span><span class="sxs-lookup"><span data-stu-id="99bcf-113">0</span></span>|<span data-ttu-id="99bcf-114">Não é um estado de ação válido</span><span class="sxs-lookup"><span data-stu-id="99bcf-114">Not a valid action state</span></span>|
|<span data-ttu-id="99bcf-115">pendente</span><span class="sxs-lookup"><span data-stu-id="99bcf-115">pending</span></span>|<span data-ttu-id="99bcf-116">1</span><span class="sxs-lookup"><span data-stu-id="99bcf-116">1</span></span>|<span data-ttu-id="99bcf-117">A ação é pendente</span><span class="sxs-lookup"><span data-stu-id="99bcf-117">Action is pending</span></span>|
|<span data-ttu-id="99bcf-118">cancelado</span><span class="sxs-lookup"><span data-stu-id="99bcf-118">canceled</span></span>|<span data-ttu-id="99bcf-119">2</span><span class="sxs-lookup"><span data-stu-id="99bcf-119">2</span></span>|<span data-ttu-id="99bcf-120">Ação foi cancelada.</span><span class="sxs-lookup"><span data-stu-id="99bcf-120">Action has been cancelled.</span></span>|
|<span data-ttu-id="99bcf-121">ativo</span><span class="sxs-lookup"><span data-stu-id="99bcf-121">active</span></span>|<span data-ttu-id="99bcf-122">3</span><span class="sxs-lookup"><span data-stu-id="99bcf-122">3</span></span>|<span data-ttu-id="99bcf-123">Ação está ativa.</span><span class="sxs-lookup"><span data-stu-id="99bcf-123">Action is active.</span></span>|
|<span data-ttu-id="99bcf-124">done</span><span class="sxs-lookup"><span data-stu-id="99bcf-124">done</span></span>|<span data-ttu-id="99bcf-125">4</span><span class="sxs-lookup"><span data-stu-id="99bcf-125">4</span></span>|<span data-ttu-id="99bcf-126">Ação concluída sem erros.</span><span class="sxs-lookup"><span data-stu-id="99bcf-126">Action completed without errors.</span></span>|
|<span data-ttu-id="99bcf-127">Falha</span><span class="sxs-lookup"><span data-stu-id="99bcf-127">failed</span></span>|<span data-ttu-id="99bcf-128">5</span><span class="sxs-lookup"><span data-stu-id="99bcf-128">5</span></span>|<span data-ttu-id="99bcf-129">Falha na ação</span><span class="sxs-lookup"><span data-stu-id="99bcf-129">Action failed</span></span>|
|<span data-ttu-id="99bcf-130">notSupported</span><span class="sxs-lookup"><span data-stu-id="99bcf-130">notSupported</span></span>|<span data-ttu-id="99bcf-131">6</span><span class="sxs-lookup"><span data-stu-id="99bcf-131">6</span></span>|<span data-ttu-id="99bcf-132">Não há suporte para a ação.</span><span class="sxs-lookup"><span data-stu-id="99bcf-132">Action is not supported.</span></span>|




