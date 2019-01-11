---
title: tipo de enum complianceState
description: Estado de conformidade.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 53b17f258f577e0842dbfc81c6341303f6b43799
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820339"
---
# <a name="compliancestate-enum-type"></a><span data-ttu-id="e15b7-103">tipo de enum complianceState</span><span class="sxs-lookup"><span data-stu-id="e15b7-103">complianceState enum type</span></span>

> <span data-ttu-id="e15b7-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e15b7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e15b7-105">Estado de conformidade.</span><span class="sxs-lookup"><span data-stu-id="e15b7-105">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="e15b7-106">Membros</span><span class="sxs-lookup"><span data-stu-id="e15b7-106">Members</span></span>
|<span data-ttu-id="e15b7-107">Membro</span><span class="sxs-lookup"><span data-stu-id="e15b7-107">Member</span></span>|<span data-ttu-id="e15b7-108">Valor</span><span class="sxs-lookup"><span data-stu-id="e15b7-108">Value</span></span>|<span data-ttu-id="e15b7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e15b7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e15b7-110">unknown</span><span class="sxs-lookup"><span data-stu-id="e15b7-110">unknown</span></span>|<span data-ttu-id="e15b7-111">0</span><span class="sxs-lookup"><span data-stu-id="e15b7-111">0</span></span>|<span data-ttu-id="e15b7-112">Desconhecido.</span><span class="sxs-lookup"><span data-stu-id="e15b7-112">Unknown.</span></span>|
|<span data-ttu-id="e15b7-113">compatível com</span><span class="sxs-lookup"><span data-stu-id="e15b7-113">compliant</span></span>|<span data-ttu-id="e15b7-114">1</span><span class="sxs-lookup"><span data-stu-id="e15b7-114">1</span></span>|<span data-ttu-id="e15b7-115">Compatível com.</span><span class="sxs-lookup"><span data-stu-id="e15b7-115">Compliant.</span></span>|
|<span data-ttu-id="e15b7-116">fora de conformidade</span><span class="sxs-lookup"><span data-stu-id="e15b7-116">noncompliant</span></span>|<span data-ttu-id="e15b7-117">2</span><span class="sxs-lookup"><span data-stu-id="e15b7-117">2</span></span>|<span data-ttu-id="e15b7-118">Dispositivo não está em conformidade e seja bloqueado para recursos corporativos.</span><span class="sxs-lookup"><span data-stu-id="e15b7-118">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="e15b7-119">conflito</span><span class="sxs-lookup"><span data-stu-id="e15b7-119">conflict</span></span>|<span data-ttu-id="e15b7-120">3</span><span class="sxs-lookup"><span data-stu-id="e15b7-120">3</span></span>|<span data-ttu-id="e15b7-121">Conflito com outras regras.</span><span class="sxs-lookup"><span data-stu-id="e15b7-121">Conflict with other rules.</span></span>|
|<span data-ttu-id="e15b7-122">erro</span><span class="sxs-lookup"><span data-stu-id="e15b7-122">error</span></span>|<span data-ttu-id="e15b7-123">4</span><span class="sxs-lookup"><span data-stu-id="e15b7-123">4</span></span>|<span data-ttu-id="e15b7-124">Erro</span><span class="sxs-lookup"><span data-stu-id="e15b7-124">Error.</span></span>|
|<span data-ttu-id="e15b7-125">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="e15b7-125">inGracePeriod</span></span>|<span data-ttu-id="e15b7-126">254</span><span class="sxs-lookup"><span data-stu-id="e15b7-126">254</span></span>|<span data-ttu-id="e15b7-127">Dispositivo não está em conformidade, mas ainda tem acesso aos recursos corporativos</span><span class="sxs-lookup"><span data-stu-id="e15b7-127">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="e15b7-128">configManager</span><span class="sxs-lookup"><span data-stu-id="e15b7-128">configManager</span></span>|<span data-ttu-id="e15b7-129">255</span><span class="sxs-lookup"><span data-stu-id="e15b7-129">255</span></span>|<span data-ttu-id="e15b7-130">Gerenciado pelo Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="e15b7-130">Managed by Config Manager</span></span>|



